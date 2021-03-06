------biu------看过的都通过-------biu------

因全文较长，本文目录如下，以方便查阅：

Part-1 云概念

Part-2 体系结构和服务保证

Part-3 Azure计算

Part-4 存储

Part-5 网络

Part-6 安全

Part-7 support

AZ-900主要考察考生对于云服务的基础知识和核心服务的理解，面向希望证明自己掌握Cloud 服务基础知识以及如何通过 Microsoft Azure 提供这些服务的考生。考试主要考察四个部分：
1. 了解Cloud概念（15%-20%）；
2. 了解核心Azure服务（30%-35%）；
3. 了解安全性、隐私、合规性和信任（25%-30%）；
4. 了解Azure定价和支持（25%-30%）。
详细的考察内容如下：
#### 了解云概念（15%-20%）：
描述使用 Cloud 服务的好处和注意事项；
描述基础架构即服务（IaaS），平台即服务（PaaS）和software as a service（SaaS）之间的差异；
描述公共 Cloud ，私有 Cloud 和混合 Cloud 模型之间的差异。
#### 了解核心Azure服务（30%-35%）：
了解核心 Azure 架构组件；
描述 Azure 中可用的一些核心产品；
描述 Azure 上可用的一些解决方案；
了解Azure管理工具。
#### 了解安全性、隐私、合规性和信任（25%-30%）：
了解 Azure 中的安全网络连接；
描述核心 Azure 身份服务；
描述 Azure 的安全工具和功能；
描述 Azure 治理方法；
了解 Azure 中的监控和报告选项；
了解 Azure 中的隐私，合规性和数据保护标准。
#### 了解Azure定价和支持（25%-30%）：
了解Azure订阅；
了解成本的规划和管理；
了解Azure提供的支持选项；
描述Azure服务水平协议（SLA）；
了解Azure中的服务生命周期。
 
学习资料:
https://docs.microsoft.com/zh-cn/learn/paths/azure-fundamentals/(中文)
https://docs.microsoft.com/en-us/learn/paths/azure-fundamentals/（英文）
本次整理只涉及AZ-900中涉及到的基本概念，更深层次的内容需要大家自己进行消化理解。

#### Part-1 云概念
1.   Cloud services have certaincharacteristics and considerations, such as:
High availability
Scalability
Elasticity
Agility
Fault tolerance
Disaster recovery
Global reach
Customer latency capabilities
Predictive cost considerations
Security
2.   在过去，公司需要购置实体房屋和基础设施，才能开办企业。开办或发展企业所需的硬件和基础设施需要大量的前期成本。云计算可以为客户提供服务，而无需大量的前期成本或设备安装时间。
这两种投资方式称为：
o  资本支出 (CapEx)：CapEx 是预先将资金花在实体基础设施上，然后逐渐从税单中扣除这笔费用。CapEx 是一种前期成本，其价值会随着时间的推移而降低。（服务器成本、网络成本、存储成本、数据中心基础设施成本等等。）
o  运营支出 (OpEx)：OpEx 是现在花钱购买服务或产品，现在为其付费。可以在同一年从税单中扣除此项费用。无前期成本。你可以在使用服务或产品时为其付费。如果需求波动位置，则OpEx极具吸引力。
3.   云部署模型
公有云:
优点
- 高可伸缩性/敏捷性 - 无需购买新的服务器即可缩放
- 即用即付定价 - 只需为使用的资源付费，无需支付 CapEx 费用
- 你不负责维护或更新硬件
- 设置和使用所需的技术知识非常少 - 可以利用云提供商的技能和专业知识来确保工作负荷的安全性和高可用性
常见用例场景是在云提供商拥有的硬件和资源上部署 Web 应用或博客站点。通过在此方案中使用公有云，云用户可以快速创建网站或博客，然后专注于维护网站，而无需担心购买、管理或维护其运行的硬件的问题。
缺点
公有云并不适合所有方案。下面是一些需要注意的缺点：
- 使用公有云可能无法满足特定的安全要求
- 公有云可能无法满足政府政策、行业标准或法律要求
- 你不拥有硬件或服务，也无法按照你的意愿管理它们
- 可能很难满足独特的业务需求，例如必须维护旧版应用程序
私有云
优点
此方法具有几个优点：
- 可以确保配置可以支持任何场景或旧版应用程序
- 你对安全性有控制能力（并承担相应责任）
- 私有云可以满足严格的安全性、合规性或法律要求
- 实现大规模经济性，并与 Azure 安全中心集成
缺点
团队迁离私有云的一些原因包括：
- 存在初始 CapEx 成本，必须购买硬件才能启动和维护
- 对设备的拥有会限制敏捷性 - 必须购买、安装和设置新硬件才能进行缩放
- 私有云需要 IT 技能和专业知识，而这些技能和知识很难获得
混合云
优点
下面是混合云的一些优点：
- 可使所有系统继续运行并保持可访问性，即使所用的操作系统或硬件已过时
- 可以灵活地在本地运行，而不是在云中运行
- 可以利用公有云提供商提供的规模效益，获得服务和资源（如果较便宜），或对自己的现有设备进行补充（如果服务和资源不是较便宜）
- 如果你需要完全控制环境，可以使用自己的设备来满足安全性、合规性或旧版方案要求
缺点
需要注意的一些问题包括：
- 这可能比选择一个部署模型更昂贵，因为它涉及一些前期的 CapEx 成本
- 设置和管理可能会更复杂
4.   云服务类型
- IaaS: Flexibility. IaaS is the most flexible cloudservice as you have control to configure and manage the hardware running yourapplication.
- PaaS: Productivity. Users can focus on applicationdevelopment only, as all platform management is handled by the cloud provider.Working with distributed teams as services is easier, as the platform isaccessed over the internet and can be made globally available more easily.
- SaaS: Pay-as-you-go pricing model. Users pay for thesoftware they use on a subscription model, typically monthly or yearly,regardless of how much they use the software.
 

![images](https://github.com/JanlenHu/OCPChinaPTSALLDOCS/blob/master/01.BLOG/images2/AZ-900考试基本知识点梳理%20%26%20Azure基础知识概要1.jpg)
 
#### Part-2 体系结构和服务保证
1.   区域是指地球上的某个地理区域，包含至少一个（但很可能是多个）数据中心，这些数据中心彼此相邻并通过一个低延迟的网络相互连接。Azure 智能地分配和控制每个区域内的资源，以确保适当平衡工作负载。（Azure is made up of datacenters located around the globe. Thesedatacenters are organized and made available to end users by country/region）
2.   Azure 将世界划分为由地缘政治边界或国家/地区边界定义的多个地域。一个Azure 地域代表一个独立市场，通常包含两个或更多个设有数据驻留和合规性边界的区域。这种划分方式具有以下几个优点。
- 地域使具有特定数据驻留和合规性要求的客户可将其数据和应用程序部署在距离其较近的位置。
- 地域保证数据驻留、主权、合规性和复原能力的要求在地域边界内得到满足。
- 通过与专用的高容量网络基础设施相连，地域具有容错能力，可承受整个区域的故障。
3.   可用性区域是 Azure 区域中的物理上独立的数据中心。
每个可用性区域都由一个或多个数据中心组成，这些数据中心都配置了独立的电源、冷却和网络设备。可用性区域被设置为_隔离边界_。如果一个区域出现故障，其他区域会继续正常工作。可用性区域通过高速专用光纤网络相连。（但并非每个区域都支持可用性区域）
4.   区域对:
在同一地域（例如美国、欧洲或亚洲）内，每个 Azure 区域始终与至少距其 300 英里外的另一区域配对。此方法适用于跨地域复制资源（例如虚拟机存储），有助于减少因自然灾害、社会动乱、电力中断或物理网络中断等事件（同时影响两个区域）造成服务中断的可能性。
5.   服务级别协议（SLA）
Azure 产品和服务的 SLA 有三个主要特征：
- 性能目标
- 运行时间和连接性保证
- 服务信用额度
6.   Azure管理选项
通常用于日常管理和交互的工具包括：
- Azure 门户，用于通过图形用户界面 (GUI) 与 Azure 交互，可以使用任何 Web 浏览器进行访问。
- Azure PowerShell 和Azure 命令行接口 (CLI)，用于与 Azure 进行基于命令行和自动化的交互。Azure PowerShell 是一个可以为 Windows PowerShell 或 PowerShell Core 安装的模块。它是跨平台版本的 PowerShell，可以在 Windows、 Linux 或macOS 上运行。Azure CLI 是一个跨平台的命令行程序，它连接到 Azure 并对 Azure 资源执行管理命令。“跨平台”意味着它可以在 Windows、Linux 或macOS 上运行。
- Azure Cloud Shell，用于基于 Web 的命令行接口。
- Azure 移动应用，用于监视和管理移动设备上的资源。
7.  Azure Policy & 策略 & 计划
Azure Policy 是 Azure 中的一项服务，用于定义、分配和管理环境中的资源标准。它可以防止创建不允许使用的资源，确保新资源应用特定设置，并对现有资源运行评估以扫描不合规的情况。
若要创建并实施 Azure Policy，需要先创建_策略定义_。每种策略定义在其特定的条件下将被强制执行。并且，在满足条件时将出现随附效果。若要应用策略，你将：
- 创建策略定义
- 将定义分配给资源作用域
- 查看策略评估结果
管理几个策略定义很容易，可一旦多起来，你就会想对它们进行整理。这时，可以用计划帮助管理。
计划可与 Azure Policy 中的策略配合使用。 计划定义是一组策略定义，可帮助你跟踪更大目标的合规性状态。即使你只有一个策略，但如果你预计随着时间推移，策略数量会增加，也建议使用计划。
 
#### Part-3 Azure计算
Azure 计算是一种按需计算服务，用于运行基于云的应用程序。它通过虚拟机和容器提供多核处理器和超级计算机等计算资源。它还提供无服务器计算，无需设置或配置基础结构即可运行应用。资源按需提供，通常可在几分钟甚至几秒内创建。只需为使用的资源付费，并且只在使用它们时付费。
有四种用于在 Azure 中执行计算的常用技术：
- 虚拟机：
虚拟机 (VM) 是物理计算机的软件模拟。它们包括虚拟处理器、内存、存储和网络资源。它们托管一个操作系统 (OS)，用户可以像使用物理计算机一样安装和运行软件。使用远程桌面客户端可以像坐在终端前面一样使用和控制虚拟机。特点：1）对操作系统 (OS) 的完全控制；2）能够运行自定义软件，3）使用自定义托管配置
- 可用性集：两个或多个VM 的逻辑分组，这些 VM 帮助确保应用程序在计划内或计划外维护期间可用。
- 虚拟机规模集：使用Azure 虚拟机规模集可以创建并管理一组完全相同的、负载均衡的 VM。
- 容器：
容器是用于运行应用程序的虚拟化环境。容器与虚拟机的共同点是它们都在主机操作系统上运行，不同之处是，容器不包括在该容器内运行的应用的操作系统。相反，容器将捆绑运行应用程序所需的库和组件，并使用运行该容器的现有主机 OS。例如，如果有五个容器在具有特定 Linux 内核的服务器上运行，则所有五个容器以及其中的应用都共享同一 Linux 内核。
Azure 支持 Docker 容器，有多种管理方法可以用来 Azure 容器。
- Azure 容器实例 (ACI)：
提供了在 Azure 中运行容器的最快且最简单的方法。无需管理任何虚拟机或配置任何其他服务。它是一种 PaaS 产品/服务，可用于上传容器并直接执行它们。
- Azure Kubernetes 服务 (AKS)：
自动化和管理大量容器及其交互方式的任务称为“业务流程”。AzureKubernetes 服务 (AKS) 是完整的面向容器的业务流程服务，包含具有多个容器的分布式体系结构。
- Azure 应用服务：
Azure 应用服务是 Azure 中的平台即服务 (PaaS) 产品/服务，为托管面向Web 的企业级应用程序而设计。在使用完全托管的平台执行基础结构维护的同时，可以满足严苛的性能、可伸缩性、安全性和合规性要求。
- 无服务器计算：
无服务器计算是一个云托管执行环境，可运行代码，但是将基础托管环境完全抽象化。创建该服务的实例以及添加代码，无需甚至不允许配置或维护基础结构。
 
#### Part-4存储
1. Azure 数据存储的一些重要优势：
- 自动备份和恢复：减轻发生任何意外故障或中断时丢失数据的风险。
- 在全球范围内复制：复制数据，防止出现任何计划内或计划外事件（例如计划性维护或硬件故障）。可选择在全球多个位置复制数据。
- 支持数据分析：支持对数据使用情况进行分析。
- 加密功能：对数据加密，使之十分安全；也可对能够访问数据的人员进行严格控制。
- 多种数据类型：Azure几乎可以存储所需的任何类型的数据。它可以处理视频文件、文本文件甚至虚拟硬盘等大型二进制文件。它还为关系数据和 NoSQL 数据提供了多种选项。
- 虚拟磁盘中的数据存储：Azure 还可在其虚拟磁盘中存储多达 8 TB 的数据。在存储大量数据（例如视频和模拟）时，这是一项重要功能。
- 存储层：存储层可根据信息的使用频率来确定数据访问的优先级。
2. Azure SQL 数据库
Azure SQL 数据库是基于最新稳定版 Microsoft SQL Server 数据库引擎的关系数据库即服务 (DaaS)。SQL 数据库是一种高性能、完全托管、可靠且安全的数据库。
3. Azure Cosmos DB
Azure Cosmos DB 是全球分布式数据库服务。它支持无架构数据，可用于生成高度响应和AlwaysOn 应用程序，以支持不断变化的数据。此功能可用于存储全球用户更新和维护的数据。 
4. Azure Blob 存储
Azure Blob 存储是非结构化的，这意味着它可以保存的数据类型没有限制。Blob 具有高度可伸缩性，应用使用 Blob 的方式与使用磁盘上的文件大致相同，例如读取和写入数据。 
5. Azure Data Lake Storage
借助 Data Lake 功能，可对数据使用情况进行分析并准备报表。Data Lake 是大型存储库，可存储结构化和非结构化数据。
6. Azure 文件存储
Azure 文件存储在云端提供完全托管的文件共享，这些共享项可通过行业标准的服务器消息块(SMB) 协议进行访问。Azure 文件共享可由云或者Windows、Linux 和 macOS 的本地部署同时装载。
7. Azure 队列
Azure 队列存储是一项可存储大量消息的服务，用户可以从世界各地的任何位置访问这些消息。
 
#### Part-5 网络
1.   虚拟网络
“虚拟网络”指的是 Azure 中逻辑隔离的网络。虚拟网络可分割为一个或多个_子网_。可借助子网在离散部分组织和保护资源。 
2.   网络安全组
网络安全组或 NSG 可以允许或拒绝流向 Azure 资源的入站网络流量。网络安全组应视为网络的云级防火墙。
3.   负载均衡器
负载均衡器在池中的每个系统之间平均分配流量。负载均衡器可帮助实现高可用性和复原。
4.   Azure应用程序网关
如果所有流量都是 HTTP 流量，则可能更好的选择是使用 Azure 应用程序网关。应用程序网关是专为 Web 应用程序设计的负载均衡器。它在传输级别 (TCP) 使用 Azure 负载均衡器，并应用复杂的基于 URL 的传递规则来支持多个高级方案。
5.   内容分发网络（ContentDelivery Network）
高效地向用户分发Web内容地分布式服务器网络。向本地用户提供内容的方法，可最大程度减少延迟。
6.   流量管理器（TrafficManager）
使用最近邻用户的DNS服务器将用户流量定向到全球分布的终结点。
7.   DNS
DNS 或域名系统是一种将用户友好名称映射到其 IP 地址的方法。可将 DNS 视为 Internet 的电话簿。
 
#### Part-6 安全
1. Azure Active Directory
Azure AD 是一种基于云的标识服务。它内置支持，可与现有本地 ActiveDirectory 同步，也可单独使用。这意味着所有应用程序，无论其位于本地、云中（包括 Office365）还是移动设备中，都可共享同一凭证。
2. 多重身份验证（MFA）
多重身份验证 (MFA) 要求通过两个或两个以上的元素进行完整的身份验证，为标识提供附加安全性。
3. 基于角色的访问控制（RBAC）
将标识直接地或通过组成员身份间接地映射至角色。将安全主体、访问权限和资源分离即可进行简单的访问管理和精细的控制。管理员可以确保授予的是最低且必需的权限。
4. 加密
- 静态加密：
静态数据是存储在物理介质上的数据。这可以是存储在服务器磁盘上的数据、存储在数据库中的数据或存储在存储帐户中的数据。无论存储机制如何，静态数据加密都可确保在没有解密密钥和机密的情况下，存储的数据不可读。
- 传输中加密：
传输中的数据是主动从一个位置移动到另一个位置的数据，例如通过 Internet 或通过专用网络。可以通过多个不同的层来处理安全传输。执行时，可以在应用程序层加密数据，然后再将其通过网络进行发送。HTTPS 是应用程序层传输中加密的示例。
5. 网络
网络安全分层方法
- 防火墙是基于每个请求的来源 IP 地址授予服务器访问权限的服务。可以创建用于指定 IP 地址范围的防火墙规则。只有来自这些已获授权的 IP 地址的客户端才能访问服务器。一般而言，防火墙规则还包括特定的网络协议和端口信息。
- 阻止分布式拒绝服务(DDoS) 攻击
将 Azure DDoS 防护与应用程序设计最佳做法相结合，可帮助防御 DDoS 攻击。DDoS 防护利用 Microsoft 全球网络的规模和弹性，为每个 Azure 区域带来 DDoS 缓解能力。Azure DDoS 防护服务通过在流量能够影响服务的可用性之前在 Azure 网络边缘监视流量，来保护Azure 应用程序。在检测到攻击的几分钟内，系统会使用 AzureMonitor 指标通知你。
6. 信息保护（AIP）
一种基于云的解决方案，可帮助组织通过应用标签来对文档和电子邮件进行分类和选择性保护。
7. Azure 高级威胁防护 （ATP）
Azure 高级威胁防护 (Azure ATP) 是一种基于云的安全解决方案，可识别、检测并帮助调查针对组织的高级威胁、泄露的标识和恶意内部操作。
 
#### Part-7 support
https://azure.microsoft.com/en-us/support/plans/
主要注意一下各个support plan的不同。
