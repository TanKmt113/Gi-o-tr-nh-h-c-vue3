# Giáo trình Vue 3 Cơ Bản

## Tuần 1: Nền tảng Web & Công cụ
| Bài | Mục tiêu                   | Nội dung chi tiết                                                                 | Thực hành                                                                                     |
|-----|----------------------------|----------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------|
| B1  | Hiểu cấu trúc web cơ bản   | • HTML5 semantic tags<br>• CSS Box Model/Flexbox/Grid<br>• Responsive design principles | Tạo trang portfolio với:<br>- Header navigation<br>- Main content section<br>- Footer với media queries |
| B2  | Nắm JS cốt lõi cho Vue     | • ES6+ (arrow functions, destructuring)<br>• Async/Await<br>• JSON manipulation         | Xây dựng BMI calculator:<br>1. Xử lý form input<br>2. Tính toán BMI<br>3. Hiển thị kết quả + phân loại |
| B3  | Tương tác DOM thuần        | • DOM querySelectors<br>• Event listeners<br>• Dynamic content updates                | Tạo todo-list:<br>- Thêm/xóa task<br>- Đánh dấu hoàn thành<br>- Lưu trữ localStorage         |
| B4  | Thiết lập môi trường Vue   | • Node.js ecosystem<br>• Vite architecture<br>• npm scripts                           | ```bash<br>npm create vite@latest vue-app --template vue<br>```<br>Cấu hình ESLint + Prettier |
| B5  | Hiểu kiến trúc Vue cơ bản  | • SFC (Single File Components)<br>• Reactivity system<br>• Virtual DOM                | Tạo component HelloWorld:<br>- Props nhận tên<br>- Button emit sự kiện<br>- Conditional rendering |

## Tuần 2: Vue 3 Cơ Bản (Options API)
| Bài | Mục tiêu                             | Nội dung chi tiết                                                                 | Thực hành                                                                                     |
|-----|--------------------------------------|----------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------|
| B6  | Sử dụng template syntax linh hoạt    | • Interpolation {{ }}<br>• Directive v-bind/v-model<br>• Dynamic classes & styles      | Form đăng ký với:<br>- Two-way binding<br>- Real-time validation<br>- Dynamic error styling   |
| B7  | Xử lý sự kiện hiệu quả               | • v-on modifiers (.stop, .prevent)<br>• Key events (.enter, .tab)<br>• Custom events     | Máy tính bỏ túi:<br>- Xử lý phép tính<br>- Hiển thị lịch sử<br>- Custom event reset           |
| B8  | Phân biệt methods/computed/watch     | • Computed caching<br>• Watch deep option<br>• Method invocation                     | Bộ đếm:<br>- Computed: tổng giá trị<br>- Watch: theo dõi thay đổi<br>- Methods: xử lý logic   |
| B9  | Hiểu vòng đời component              | • created: fetch data<br>• mounted: DOM access<br>• unmounted: cleanup             | Tích hợp thư viện ngoài (Chart.js):<br>- Khởi tạo biểu đồ trong mounted<br>- Destroy trong unmounted |
| B10 | Xây dựng component tái sử dụng       | • Prop validation<br>• Slot mechanisms (default/named)<br>• Fallthrough attributes | Card component:<br>- Nhận dữ liệu qua props<br>- Slot cho nội dung tùy biến<br>- CSS scoped    |

## Tuần 3: Composition API
| Bài | Mục tiêu                       | Nội dung chi tiết                                                                 | Thực hành                                                                                     |
|-----|--------------------------------|----------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------|
| B11 | Chuyển đổi sang Composition API | • setup() syntax<br>• ref vs reactive<br>• toRefs destructuration                     | Refactor counter app:<br>- Tách logic thành hàm<br>- Sử dụng reactive object<br>- toRefs cho template |
| B12 | Theo dõi phản ứng dữ liệu       | • watch vs watchEffect<br>• Immediate option<br>• Effect cleanup                   | Search component:<br>- watchEffect tìm kiếm real-time<br>- watch cho tham số URL<br>- Debounce |
| B13 | Sử dụng computed hiệu quả       | • Computed với ref<br>• Setter computed<br>• Performance optimization               | Giỏ hàng:<br>- Tính tổng tiền computed<br>- Filter sản phẩm<br>- Sort theo giá computed       |
| B14 | Tái sử dụng logic               | • Composables pattern<br>• useCounter/useFetch<br>• Shared state                   | Tạo useFetch():<br>- Xử lý data/loading/error<br>- Tái sử dụng cho API endpoints              |
| B15 | So sánh Options vs Composition  | • Ưu/nhược điểm<br>• Migration strategy<br>• Hybrid approach                        | Refactor component từ Tuần 2:<br>- Chuyển sang setup()<br>- So sánh độ phức tạp code          |

## Tuần 4: Vue Router
| Bài | Mục tiêu                     | Nội dung chi tiết                                                                 | Thực hành                                                                                     |
|-----|------------------------------|----------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------|
| B16 | Thiết lập định tuyến cơ bản   | • createRouter<br>• Route configuration<br>• History mode                         | Tạo SPA với:<br>- Trang chủ (/)<br>- Giới thiệu (/about)<br>- Liên hệ (/contact)               |
| B17 | Xử lý route động             | • Dynamic segments (:id)<br>• Nested routes<br>• Route meta fields               | Product detail page:<br>- /products/:id<br>- Nested /reviews<br>- Meta: requiresAuth          |
| B18 | Điều hướng trong ứng dụng     | • router-link<br>• Programmatic navigation<br>• Active link styling              | Navbar component:<br>- router-link với exact-active-class<br>- Navigation guard chuyển hướng   |
| B19 | Bảo vệ route                 | • Global guards<br>• Per-route guards<br>• Authentication flow                   | Tạo login system:<br>- beforeEach kiểm tra auth<br>- Redirect đến /login nếu chưa đăng nhập    |
| B20 | Tối ưu tải trang             | • Lazy loading components<br>• Dynamic imports<br>• Code splitting               | ```js<br>component: () => import('./views/Admin.vue')<br>```<br>Phân tích bundle với vite-plugin-visualizer |

## Tuần 5: Pinia State Management
| Bài | Mục tiêu                     | Nội dung chi tiết                                                                 | Thực hành                                                                                     |
|-----|------------------------------|----------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------|
| B21 | Thiết lập Pinia cơ bản       | • createPinia()<br>• Store definition<br>• Setup vs Options stores               | Tạo auth store:<br>- State: user, token<br>- Getters: isLoggedIn<br>- Actions: login/logout   |
| B22 | Quản lý state tập trung      | • State reactivity<br>• Getters như computed<br>• Async actions                 | Giỏ hàng store:<br>- Thêm/xóa sản phẩm<br>- Tính tổng tiền getter<br>- Async checkout action  |
| B23 | Sử dụng store trong component | • useStore()<br>• StoreToRefs<br>• State subscription                          | Hiển thị giỏ hàng:<br>- Truy cập store từ component<br>- Auto-update khi state thay đổi       |
| B24 | Modular stores               | • Store composition<br>• Cross-store actions<br>• useUserStore/useCartStore    | Tích hợp stores:<br>- UserStore: thông tin user<br>- CartStore: sử dụng userId từ UserStore   |
| B25 | Duy trì state                | • Pinia plugins<br>• localStorage persistence<br>• Hydration                   | Tạo plugin:<br>- Lưu cart vào localStorage<br>- Khôi phục state khi refresh<br>- Serialization |

## Tuần 6: API & UI Framework
| Bài | Mục tiêu                     | Nội dung chi tiết                                                                 | Thực hành                                                                                     |
|-----|------------------------------|----------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------|
| B26 | Giao tiếp REST API           | • Axios interceptors<br>• Base configuration<br>• RESTful conventions            | Tạo api service:<br>- GET/POST/PUT/DELETE<br>- Xử lý headers<br>- Tái sử dụng instance        |
| B27 | Xử lý trạng thái không đồng bộ | • Loading states<br>• Error handling<br>• Global progress bar                  | Hiển thị skeleton loader:<br>- Component loading state<br>- Global error handler<br>- Retry logic |
| B28 | Thiết lập UI framework       | • Vuetify/Element Plus<br>• Theme customization<br>• Responsive utilities       | Cài đặt Vuetify:<br>```bash<br>npm install vuetify@^3<br>```<br>Customize theme màu sắc       |
| B29 | Sử dụng component UI         | • Data tables<br>• Form controls<br>• Modal dialogs                            | Dashboard admin:<br>- Table CRUD operations<br>- Filter/sort dữ liệu<br>- Modal xác nhận xóa  |
| B30 | Form validation              | • VeeValidate + Yup<br>• Schema validation<br>• Error messages localization    | Form đăng ký:<br>- Validation real-time<br>- Schema Yup phức tạp<br>- Hiển thị lỗi đa ngôn ngữ |

## Tuần 7: Tối ưu hiệu năng
| Bài | Mục tiêu                     | Nội dung chi tiết                                                                 | Thực hành                                                                                     |
|-----|------------------------------|----------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------|
| B31 | Tối ưu trải nghiệm người dùng | • Suspense<br>• Lazy loading<br>• KeepAlive component                           | Sử dụng Suspense:<br>- Loading fallback<br>- Lazy load heavy components<br>- KeepAlive cho tabs |
| B32 | Quản lý component nâng cao   | • Dynamic components<br>• Teleport<br>• Component registration                 | Modal system:<br>- Teleport vào body<br>- Dynamic component type<br>- Global registration     |
| B33 | Xử lý danh sách lớn          | • Virtual scrolling<br>• Pagination<br>• Infinite loading                      | Danh sách 10,000 sản phẩm:<br>- vue-virtual-scroller<br>- Server-side pagination<br>- Load more |
| B34 | Responsive design            | • Mobile-first approach<br>• CSS media queries<br>• Tailwind responsive classes | Xây dựng layout responsive:<br>- Grid thay đổi theo breakpoints<br>- Ẩn/hiện menu mobile      |
| B35 | Debug & performance          | • Vue DevTools<br>• Performance audits<br>• Bundle analysis                    | Phân tích performance:<br>- Lighthouse audit<br>- Xác định bottlenecks<br>- Sử dụng memoization |

## Tuần 8: Dự án thực chiến
| Bài | Mục tiêu                     | Nội dung chi tiết                                                                 | Thực hành                                                                                     |
|-----|------------------------------|----------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------|
| B36 | Phân tích yêu cầu            | • Feature planning<br>• Architecture design<br>• Tech stack selection            | Chọn project e-commerce:<br>- Sơ đồ use-case<br>- Component tree<br>- API specification       |
| B37 | Triển khai UI + routing      | • Layout system<br>• Route structure<br>• Theming                               | Xây dựng:<br>- Main layout<br>- Product/Checkout routes<br>- Dark mode toggle                 |
| B38 | Tích hợp API + quản lý state | • API services<br>• Pinia stores<br>• State hydration                           | Kết nối backend:<br>- Auth store<br>- Product store<br>- Cart synchronization                 |
| B39 | Xử lý form + validation      | • Complex forms<br>• Multi-step workflows<br>• Error handling                   | Checkout flow:<br>- 3 bước thanh toán<br>- Address validation<br>- Payment method selection  |
| B40 | Build + deployment           | • Vite production build<br>• Environment variables<br>• CI/CD pipeline          | ```bash<br>npm run build<br>```<br>Deploy lên Netlify:<br>- Config redirects<br>- Environment vars |
