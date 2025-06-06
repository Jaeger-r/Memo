# Memo
项目完整目录结构
com.example.memoapp/
├── MainActivity.kt                            // 应用入口，处理导航
│
├── data/                                      // 数据层
│   ├── model/
│   │   ├── User.kt                            // 用户数据模型
│   │   └── Memo.kt                            // 备忘录数据模型
│   │
│   ├── dao/
│   │   └── MemoDao.kt                         // Room DAO 接口
│   │
│   ├── database/
│   │   └── MemoDatabase.kt                    // Room 数据库实例
│   │
│   ├── repository/
│   │   ├── UserRepository.kt                  // 登录状态相关逻辑
│   │   └── MemoRepository.kt                  // 备忘录增删改查逻辑
│   │
│   └── prefs/
│       └── UserPrefs.kt                       // 登录状态的 SharedPreferences 工具类
│
├── ui/                                        // 界面层
│   ├── login/
│   │   ├── LoginActivity.kt                   // 登录界面
│   │   └── LoginViewModel.kt                 // 登录 ViewModel
│   │
│   ├── memo/
│   │   ├── MemoListActivity.kt                // 备忘录列表页面
│   │   ├── MemoDetailActivity.kt              // 备忘录详情/编辑页面
│   │   └── MemoViewModel.kt                   // 备忘录 ViewModel
│   │
│   └── adapter/
│       └── MemoAdapter.kt                     // RecyclerView 适配器
│
├── util/
│   └── ViewModelFactory.kt                    // ViewModel 工厂类，用于注入依赖
│
├── res/
│   ├── layout/                                // XML 布局文件
│   │   ├── activity_login.xml
│   │   ├── activity_memo_list.xml
│   │   ├── activity_memo_detail.xml
│   │   └── item_memo.xml
│   │
│   └── values/
│       └── strings.xml
│
└── AndroidManifest.xml
