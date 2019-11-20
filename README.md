[github源码地址]([https://github.com/guorenqing/iOSCodeSnippet](https://github.com/guorenqing/iOSCodeSnippet)
)

#使用方式
1.下载源码
```
git clone git@github.com:guorenqing/iOSCodeSnippet.git
```
2.打开Xcode代码片段存放目录
```
open ~/Library/Developer/Xcode/UserData/CodeSnippets
```
3.把下载下来的代码片段文件复制到上一步打开的目录下，注意只复制文件，不要把文件夹复制过去
# 快捷键
|代码片段|快捷键|说明|
| ------------- |---------------|-------------|
|@property (copy, nonatomic) NSString *<#name#>;|@string|字符串属性|
|@property (copy, nonatomic) NSArray *<#name#>;|@array|数组属性|
|@property (copy, nonatomic) NSDictionary *<#name#>;|@dict|字段属性|
|@property (copy, nonatomic) NSSet *<#name#>;|@set|集合属性|
|@property (strong, nonatomic) NSMutableString *<#name#>;|@mstring|可变字符串属性|
|@property (strong, nonatomic) NSMutableArray  *<#name#>;|@marray|可变数组属性|
|@property (strong, nonatomic) NSMutableDictionary *<#name#>;|@mdict|可变字典属性|
|@property (strong, nonatomic) NSMutableSet *<#name#>;|@mset|可变集合属性|
|@property (assign, nonatomic) <#type#> <#name#>;|@assign|基本类型属性|
|@property (strong, nonatomic) <#type#> *<#name#>;|@strong|strong对象属性|
|@property (copy, nonatomic) <#type#> *<#name#>;|@copy|copy对象属性|
|@property (weak, nonatomic) <#type#> *<#name#>;|@weak|weak对象属性|
|NSLog(@"<#Log#>");|@log|日志打印|
|__weak typeof(self) weakSelf = self;|@weakself|weakSelf|
|__strong typeof(<#weakSelf#>) strongSelf = <#weakSelf#>;|@strongself|strongSelf|
|static const NSInteger <#name#> = <#value#>;|@staticint|整形常量定义|
|static const CGFloat <#name#> = <#value#>;|@staticfloat|浮点型常量定义|
|static const NSString *<#name#> = <#value#>;|@staticstring|字符串常量定义|
|#pragma mark - -------------------Lifecycle--------------------|@lifecycle|生命周期分割线|
|#pragma mark - -------------------Public--------------------|@public|公开方法分割线|
|#pragma mark - -------------------Private--------------------|@private|私有方法分割线|
|#pragma mark - -------------------Setters--------------------|@setters|setters方法分割线|
|#pragma mark - -------------------Getters--------------------|@getters|getters方法分割线|
|#pragma mark - -------------------EventCallback--------------------|@eventcallback|事件回调方法分割线|
|dispatch_async(dispatch_get_global_queue(DISPATCH_QUEUE_PRIORITY_DEFAULT, 0), ^{<#code#>});|@gcdglobal|GCD 异步线程调用 |
|dispatch_async(dispatch_get_main_queue(), ^{<#code#>});||GCD main线程调用|
|UIButton *button = [[UIButton alloc] init];button.backgroundColor = [UIColor <#backgroundColor#>];button.titleLabel.font = [UIFont <#font#>];[button setTitle:<#title#> forState:UIControlStateNormal];[button setTitleColor:[UIColor <#titleColor#>] forState:UIControlStateNormal];[button addTarget:self action:@selector(buttonClicked:) forControlEvents:UIControlEventTouchUpInside];[<#view#> addSubview:button];|@buttoninit|按钮初始化|
|UIButton *borderButton = [[UIButton alloc] init];borderButton.layer.borderColor = [UIColor <#color#>].CGColor;borderButton.layer.borderWidth = <#borderWidth#>;borderButton.titleLabel.font = [UIFont <#font#>];borderButton.clipsToBounds = YES;borderButton.layer.cornerRadius = <#cornerRadius#>;borderButton.backgroundColor = [UIColor <#backgroundColor#>];[borderButton setTitleColor:[UIColor <#titleColor#>] forState:UIControlStateNormal];[borderButton setTitle:<#title#> forState:UIControlStateNormal];[borderButton addTarget:self action:@selector(borderButtonClicked:) forControlEvents:UIControlEventTouchUpInside];[<#code#> addSubview:borderButton];|@borderbutton|带描边按钮初始化|
|UILabel *label = [[UILabel alloc] init];label.font = [UIFont <#font#>];label.text = <#text#>label.textColor = [UIColor <#textColor#>];label.textAlignment = NSTextAlignmentCenter;label.backgroundColor = [UIColor clearColor];[<#view#> addSubview:label];|@labelinit|label初始化|
|UITableView *tableView = [[UITableView alloc] initWithFrame:CGRectZero style:UITableViewStylePlain];if(@available(iOS 11.0, *)) {tableView.contentInsetAdjustmentBehavior =UIScrollViewContentInsetAdjustmentNever;}[tableView registerClass:[<#classCell#> class] forCellReuseIdentifier:<#kReuseIdentifier#>];tableView.separatorStyle = UITableViewCellSeparatorStyleNone;tableView.keyboardDismissMode = UIScrollViewKeyboardDismissModeOnDrag;tableView.dataSource = self;tableView.delegate = self;|@tableinit|tableview初始化|



