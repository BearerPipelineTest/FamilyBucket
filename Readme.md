﻿## 微服务全家桶FamilyBucket应用框架
`FamilyBucket` 是一个集合多个组件应用形成的微服务一体化的全套应用框架。  

各组件源码： https://github.com/q315523275/FamilyBucket  
UI源码： https://github.com/q315523275/FamilyBucket-UI  
部分服务源码： https://github.com/q315523275/FamilyBucket-Server  
博客园地址： https://www.cnblogs.com/tianxiangzhe/p/10212337.html  
Nuget： Bucket.XXX  

---
### 特性
* 没啥特性

## 各组件矩阵
<table>
<thead>
<tr>
<th align="center">组件</th>
<th align="center">状态</th>
<th>说明</th>
</tr>
</thead>
<tbody>
<tr>
<td align="center" style="white-space:nowrap;"><a href="https://github.com/q315523275/FamilyBucket/tree/master/src/ApiGateway" title="微服务网关">微服务网关</a></td>
<td align="center" style="white-space:nowrap;">维护中</td>
<td>使用<a href="https://github.com/ThreeMammals/Ocelot" title="ocelot">ocelot</a>服务网关，扩展配置存储方式、子服务dotnetty通信</td>
</tr>
<tr>
<td align="center" style="white-space:nowrap;"><a href="https://github.com/q315523275/FamilyBucket/tree/master/src/Authorize" title="认证授权">认证授权组件</a></td>
<td align="center" style="white-space:nowrap;">维护中</td>
<td>jwt无状态认证方式，动态权限控制</td>
</tr>
<tr>
<td align="center" style="white-space:nowrap;"><a href="https://github.com/q315523275/FamilyBucket/tree/master/src/Cache" title="缓存组件">缓存组件</a></td>
<td align="center" style="white-space:nowrap;">维护中</td>
<td>多种缓存方式实现，本地缓存、redis缓存</td>
</tr>
<tr>
<td align="center" style="white-space:nowrap;"><a href="https://github.com/q315523275/FamilyBucket/tree/master/src/Config" title="配置中心">配置中心</a></td>
<td align="center" style="white-space:nowrap;">维护中</td>
<td>提供系统组件、业务等配置信息获取</td>
</tr>
<tr>
<td align="center" style="white-space:nowrap;"><a href="https://github.com/q315523275/FamilyBucket/tree/master/src/ErrorCode" title="错误码">错误码</a></td>
<td align="center" style="white-space:nowrap;">维护中</td>
<td>提供系统错误、业务错误等错误码对外的描述信息获取</td>
</tr>
<tr>
<td align="center" style="white-space:nowrap;"><a href="https://github.com/q315523275/FamilyBucket/tree/master/src/EventBus" title="事件总线">事件总线</a></td>
<td align="center">维护中</td>
<td>使用RabbitMQ实现，可用于分布式事务</td>
</tr>
<tr>
<td align="center" style="white-space:nowrap;"><a href="https://github.com/q315523275/FamilyBucket/tree/master/src/HangFire/Bucket.HangFire.Server" title="分布式调度任务">分布式调度任务</a></td>
<td align="center" style="white-space:nowrap;">使用中</td>
<td>使用Hangfire分布式调度系统</td>
</tr>
<tr>
<td align="center" style="white-space:nowrap;"><a href="https://github.com/q315523275/FamilyBucket/tree/master/src/Listener" title="组件监听">命令监听</a></td>
<td align="center" style="white-space:nowrap;">维护中</td>
<td>使用Redis、Zookeeper实现命令监听，用于组件命令接收</td>
</tr>
<tr>
<td align="center" style="white-space:nowrap;"><a href="https://github.com/q315523275/FamilyBucket/tree/master/src/Logging" title="日志收集">日志收集</a></td>
<td align="center" style="white-space:nowrap;">维护中</td>
<td>对原生日志组件实现扩展，支持Log4Net、NLog、自定义日志MQ传输(扩展告警系统)</td>
</tr>
<tr>
<td align="center" style="white-space:nowrap;"><a href="https://github.com/q315523275/FamilyBucket/tree/master/src/ORM" title="ORM">ORM</a></td>
<td align="center" style="white-space:nowrap;">维护中</td>
<td>基于<a href="https://github.com/sunkaixuan/SqlSugar" title="SqlSugar">SqlSugar</a>实现多库读写分离、数据仓储</td>
</tr>
<tr>
<td align="center" style="white-space:nowrap;"><a href="https://github.com/q315523275/FamilyBucket/tree/master/src/Rpc" title="RPC">RPC</a></td>
<td align="center" style="white-space:nowrap;">升级中</td>
<td>基于DotNetty实现Rpc应用(网关通信扩展)，gRpc连接管理</td>
</tr>
<tr>
<td align="center" style="white-space:nowrap;"><a href="https://github.com/q315523275/FamilyBucket/tree/master/src/ServiceDiscovery" title="服务发现">服务发现</a></td>
<td align="center" style="white-space:nowrap;">维护中</td>
<td>基于Consul实现服务发现、自动注册注销，服务负载计算</td>
</tr>
<tr>
<td align="center" style="white-space:nowrap;"><a href="https://github.com/q315523275/FamilyBucket/tree/master/src/SkyAPM" title="链路追踪">链路追踪</a></td>
<td align="center" style="white-space:nowrap;">维护中</td>
<td>请求链路追踪，由于资源关系对SkyAPM net客户端进行部分修改</td>
</tr>
<tr>
<td align="center" style="white-space:nowrap;"><a href="https://github.com/q315523275/FamilyBucket/tree/master/src/Utility" title="工具组件">工具组件</a></td>
<td align="center" style="white-space:nowrap;">维护中</td>
<td>常用工具类、验证码、拼音、分词</td>
</tr>
<tr>
<td align="center" style="white-space:nowrap;"><a href="https://github.com/q315523275/FamilyBucket/tree/master/src/WebSocket" title="WebSocket">WebSocket</a></td>
<td align="center" style="white-space:nowrap;">维护中</td>
<td>原生WebSocket扩展实现，易于扩展与自定义</td>
</tr>
<tr>
<td align="center" style="white-space:nowrap;">告警系统</td>
<td align="center" style="white-space:nowrap;">未开放</td>
<td>应用异常实时告警系统，多大屏展示、多种通知方式</td>
</tr>
<tr>
<td align="center" style="white-space:nowrap;">应用监控</td>
<td align="center" style="white-space:nowrap;">开发中</td>
<td>应用对应cup、内存、gc、http、并发、异常等数据监控与上报</td>
</tr>
<tr>
<td align="center" style="white-space:nowrap;"><a href="https://github.com/q315523275/FamilyBucket/tree/master/src/AspNetCore/Bucket.AspNetCore" title="AspNetCode">AspNetCode应用组件</a></td>
<td align="center" style="white-space:nowrap;">升级中</td>
<td>应用程序组件，用户上下文、健康检查接口、Controller基类、批量注册、全局异常拦截、ip白名单访问、模型验证、限速限流、熔断降级等持续开发中...</td>
</tr>
<tr>
<td align="center" style="white-space:nowrap;"><a href="https://github.com/q315523275/FamilyBucket-Server" title="框架管理">框架后台管理</a></td>
<td align="center" style="white-space:nowrap;">升级中</td>
<td>管理框架信息，网关监控路由配置、应用监控与查询管理、配置中心管理、错误码管理、链路监控与管理、日志管理、通用后台功能管理等</td>
</tr>
</tbody>
</table>

---
## 各组件使用
webapi与控制台使用示例，源码： https://github.com/q315523275/FamilyBucket/tree/master/src/Sample

```csharp
        /// <summary>
        /// 配置服务
        /// </summary>
        public void ConfigureServices(IServiceCollection services)
        {
            // 添加全家桶服务
            services.AddFamilyBucket(familyBucket =>
            {
                // 添加AspNetCore基础服务
                familyBucket.AddAspNetCore();
                // 添加授权认证
                familyBucket.AddApiJwtAuthorize().UseAuthoriser(builder => { builder.UseMySqlAuthorize(); });
                // 添加数据ORM、数据仓储
                familyBucket.AddSqlSugarDbContext().AddSqlSugarDbRepository();
                // 添加错误码服务
                familyBucket.AddErrorCodeServer();
                // 添加配置服务
                familyBucket.AddConfigServer();
                // 添加事件驱动
                familyBucket.AddEventBus(builder => { builder.UseRabbitMQ(); });
                // 添加服务发现
                familyBucket.AddServiceDiscovery(builder => { builder.UseConsul(); });
                // 添加负载算法
                familyBucket.AddLoadBalancer();
                // 添加事件队列日志和告警信息
                familyBucket.AddLogEventTransport();
                // 添加链路追踪
                familyBucket.AddBucketSkyApmCore().UseEventBusTransport();
                // 添加缓存组件
                familyBucket.AddCaching(build =>
                {
                    build.UseInMemory("default");
                    build.UseStackExchangeRedis(new Caching.StackExchangeRedis.Abstractions.StackExchangeRedisOption
                    {
                        Configuration = "10.10.188.136:6379,allowadmin=true",
                        DbProviderName = "redis"
                    });
                });
                // 添加工具组件
                familyBucket.AddUtil();
                // 添加组件定时任务
                familyBucket.AddAspNetCoreHostedService(builder => { builder.AddConfig().AddErrorCode().AddAuthorize(); });
                // 添加组件任务订阅
                familyBucket.AddListener(builder => { builder.UseRedis().AddAuthorize().AddConfig().AddErrorCode(); }); // builder.UseZookeeper();
                // 添加应用批量注册
                familyBucket.BatchRegisterService(Assembly.Load("Bucket.Demo.Repository"), "Repository", ServiceLifetime.Scoped);
                // 添加DotNetty_Rpc使用
                familyBucket.AddRpcCore().UseDotNettyTransport().UseMessagePackCodec().AddClientRuntime().AddServiceProxy(); //.UseProtoBufferCodec()
            });
            // 添加过滤器
            services.AddMvc(option => { option.Filters.Add(typeof(WebApiActionFilterAttribute)); }).AddJsonOptions(options =>
            {
                options.SerializerSettings.ContractResolver = new DefaultContractResolver();
                options.SerializerSettings.DateFormatString = "yyyy-MM-dd HH:mm:ss.fff";
            }).SetCompatibilityVersion(CompatibilityVersion.Version_2_2);
            // 添加接口文档
            services.AddSwaggerGen(c =>
            {
                c.SwaggerDoc("v1", new Info { Title = "微服务全家桶接口服务", Version = "v1" });
                c.IncludeXmlComments(Path.Combine(AppContext.BaseDirectory, "Bucket.WebApi.xml"));
                c.CustomSchemaIds(x => x.FullName);
                // Swagger验证部分
                c.AddSecurityDefinition("Bearer", new ApiKeyScheme { In = "header", Description = "请输入带有Bearer的Token", Name = "Authorization", Type = "apiKey" });
                c.AddSecurityRequirement(new Dictionary<string, IEnumerable<string>> { { "Bearer", Enumerable.Empty<string>() } });
            });
            // 添加HttpClient管理
            services.AddHttpClient();
            // 添加业务组件注册

            // 添加事件消息
            RegisterEventBus(services);
            // 注册调度任务
            RegisterScheduler(services);
        }
```


---
## 性能与稳定
* 追求极限性能其实不应该使用微服务框架，独立应用对外提供服务最好
* 网关ocelot虽然有很多功能，但是尽量只当作路由来用不要把过多功能放在网关应用，目前平均一个请求2ms左右延时
* 提供一个高可用的服务涉及到很多很多，一定要预防好级联雪崩情况
* 太多了

---
## VNext
* 灰度发布方案
* 
