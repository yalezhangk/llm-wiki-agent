---
title: "Overview"
type: synthesis
tags: []
sources: [2-smart-hvx-intelligent-medium-voltage-circuit-breaker, 3-smart-hvx-intelligent-medium-voltage-circuit-breaker-solution-overview-single-page, hvx-manual, pmb-easy-brochure, pmb-easy-johnson-v1, smart-hvx-product-introduction-v3-4, smart-hvx-product-pmb-introduction, dnf7-indoor-ac-metal-enclosed-switchgear-2025-4-10, gma-medium-voltage-primary-gas-insulated-switchgear-v1-5, gm-airset-medium-voltage-primary-gas-insulated-switchgear-v1-1, gma-air-c4c-digital-implement-20191204, gma-nrjed311328en-1017, mvnex-medium-voltage-metal-clad-switchgear, pix-50ka-catalogue-en, pix-catalogue-indoor-ac-metal-enclosed-switchgear, pix550-catalogue, pix500-catalogue-armored-metal-enclosed-switchgear, pix-indoor-ac-metal-enclosed-switchgear-v8-breaker-parameter-revision, wig-high-speed-rail-smart-switchgear-jiaoda-yunda-protection-pasific-window, gha-gas-insulated-switchgear-presentation-vers-06-englisch, gha-nrjcat18789en-0318]
last_updated: 2026-06-04
---

# Overview

当前 wiki 的首个来源是 [[SmartHVX]] 产品样本，它把 [[施耐德电气]] 的中压断路器能力包装为一个面向 [[数字化中压运维]]、数字化配电和 [[主动运维]] 的解决方案。资料显示，[[HVX]] 是机械与电气基础平台，而 [[温度智能监测]]、[[配柜智能监测]]、[[二次元件智能监测]] 和 [[PMBEasy]] 则构成智能化增量价值。

从产品组合上看，当前知识库已经有一个清晰结构：基础测温型解决就地温度可视化，标准测温型补上本地/远程接入能力，智能型进一步覆盖机械状态和二次元件健康。整体叙事依附于 [[EcoStruxure]] 架构，强调通过状态监测、边缘显示和趋势分析提升可靠性、运维效率与成本效益。

第二份来源《方案总览》补充了更清楚的方案拓扑视图，明确了 [[ZBRN32]]、[[Link150]]、[[BMM]]、[[千里眼]] 与 [[PMBEasy]] 在 Smart HVX 体系中的位置。现在 wiki 对 Smart HVX 的理解已经从“单一产品能力说明”扩展到“带本地显示、云端显示和接入链路的整体运维方案”。

第三份来源《HVX说明书》则把知识重心进一步下探到 [[HVX]] 平台本体，补充了额定电压等级、模块化型号、[[真空灭弧室]]、[[全固封极柱]]、二次装置、订货表和外形尺寸等工程信息。现在 wiki 既有 Smart HVX 的智能化方案视角，也开始具备 HVX 设备本体的选型与结构认知。

第四份来源《PMB Easy样本》则把 [[PMBEasy]] 从“Smart HVX 方案里的一个模块”升级成了独立设备对象，补充了单机版/全站版定位、具体物料号、接口、电源、柜宽适配和安装开孔尺寸。现在 wiki 对 Smart HVX 体系的理解已经形成三层：[[HVX]] 设备平台层、[[PMBEasy]] 边缘运维层，以及以 [[千里眼]] 为代表的远程展示层。

第五份来源《PMB Easy 演示稿》与 PMB Easy PDF 样本高度重合，更多起到交叉验证作用，确认了 PMB Easy 的功能边界、部署方式和安装建议，而没有引入明显相反信息。

第六份来源《Smart HVX 产品介绍 V3.4》把前述知识重新组织成销售与应用叙事，补充了 [[测温技术对比]]、可靠性承诺、状态检修效率依据、[[千里眼]] 运维工时对比和典型配电房方案。它让 wiki 对 Smart HVX 的理解从“有哪些模块”进一步扩展到“这些模块如何支撑可靠性、效率和降本的商业论证”。

第七份来源《Smart HVX & PMBox 介绍》进一步把 [[PMBEasy]] 与 [[PMBox]] 区分开：PMB Easy 更贴近 Smart HVX 的单柜/全站断路器显示和主动运维，PMBox 则是 [[EcoStruxure]] Power 边缘控制层的站室级产品，覆盖资产管理、状态监测、预测性维护、3D 站室视图、局部放电分析和历史数据查询。

第八份来源《DNF7 户内交流金属封闭开关设备》把知识库从断路器和运维单元扩展到完整中压开关柜层。[[DNF7]] 是 40.5kV 户内交流 [[金属封闭开关设备]]，强调 LSC2B 运行连续性、PM 级金属隔板、IAC AFLR 31.5kA/1s [[内部电弧防护]]、[[HVX]] 真空断路器，以及接入 [[EcoStruxure]]、[[PMBox]]、[[PMBEasy]] 和千里眼资产顾问的智能化方案。

第九份来源《GMA 中压一次气体绝缘开关柜 产品目录 V1.5》补充了另一条开关柜产品线：[[GMA]] 是 12/24kV 中压一次 [[气体绝缘开关柜]]，采用 SF6 密封气室、固体绝缘母线、模块化扩展和插接式快速安装。它与 DNF7 并列扩展了 wiki 的开关柜知识边界：DNF7 偏 40.5kV 空气绝缘，GMA 偏 12/24kV 气体绝缘紧凑方案。

第十份来源《GM AirSeT 中压一次气体绝缘开关柜 产品目录 V1.1》进一步细化了气体绝缘路线的环保分支。[[GMAirSeT]] 与 GMA 在柜型结构和模块化方案上高度相似，但采用干燥空气/环保气体替代 SF6，面向碳达峰、碳中和和低 GWP 诉求，同时保留 IAC AFLR 31.5kA/1s、IP67 气室和现场无需气体操作等工程特征。

第十一份来源《GMA Air C4C Digital Implement》不是新产品目录，而是数字化实施清单。它补充了 GMA Air / GM AirSeT 的具体监测对象：IED 保护与计量、断路器电气特性、[[气室监测]]、电缆侧温升、RFID/Zigbee、TH110/TH110-R/CL110/SD20 传感器线索，以及 [[局部放电监测]]。

第十二份来源《GMA Gas-insulated Switchgear Catalog 2017》补充了英文国际版 GMA 目录视角，给出 up to 24kV、2500A、31.5kA 的更宽参数范围，并强调 450mm 宽馈线柜、IAC AFL 1s 标配/AFLR 可选、sealed pressure system、IoT/Smart Grid ready 和 [[EcoStruxure]] ready solutions。它与中文 GMA 目录在额定电流范围上存在版本/市场口径差异，后续选型时需要按具体目录版本确认。

第十三份来源《MVnex 中压金属铠装开关柜》补充了 12kV 空气绝缘 [[金属铠装开关设备]] 路线。[[MVnex]] 产品族覆盖标准型、550 紧凑型、500 超紧凑型和 Smart MVnex 智能型：标准型可达 4000A、40kA，550/500 面向配电室小型化，Smart MVnex 则把 TH110、Easergy P3、VAMP、主动运维智能单元和 [[千里眼]] 组合成智能中压开关柜方案。

第十四份来源《PIX 50kA Catalogue EN》进一步补强了 [[空气绝缘开关设备]] 路线。[[PIX]] 目录给出 17.5kV、50kA、4000A 和 [[HVX]] embedded pole 的高性能口径，采用 LSC2B-PM 隔室结构，内部电弧能力达到 IAC AFLR 50kA/1s，并把 Easergy P3/P5、VAMP、TH110、CL110、Substation Monitoring Device、HMI、SCADA/Services 和云端应用组合进 [[EcoStruxure]] ready 的数字化运维链路。它与 [[MVnex]] 不是冲突关系，而是同属空气绝缘/金属铠装方向下不同参数段和应用场景的产品分支。

第十五份来源《PIX 户内交流金属封闭开关设备 产品目录》把 [[PIX]] 的中文市场口径补齐：PIX 被定义为铠装移开式户内交流 [[金属封闭开关设备]]，覆盖 PIX-12kV、PIX-24kV、PIX-M 接触器柜和 PIX-Gen 发电机出口断路器柜。中文目录显示，PIX-12kV 可覆盖 630A~4000A、20kA~50kA，PIX-Gen 可达 5000A/6300A 和 63kA；PIX-24kV 覆盖 630A~4000A、20kA~40kA。它还补充了四隔室结构、五防联锁、泄压通道、[[HVX]]、VAH、CVX、ESW、MiCOM、一次方案代号、订货资料和安装基础要求。与英文 PIX 目录相比，中文目录更像工程选型和订货安装手册，英文目录更偏国际版高性能/数字化宣传口径。

第十六份来源《PIX550 中置式金属封闭开关设备 产品目录》把 [[PIX]] 产品族的小型化分支单独展开。[[PIX550]] 是 PIX 旗下尺寸最小的 12kV 中置式 [[金属封闭开关设备]]，柜宽 550mm，额定电流 ≤1250A，短时耐受/开断能力 ≤31.5kA，配装 [[HVX]] 固封式真空断路器手车。它的价值不在高短路电流，而在小型化、柜前维护、靠墙/背靠背/面对面安装和与其他 PIX 柜直接拼柜，适合商业及工业建筑、房地产、数据中心等配电空间敏感场景。

第十七份来源《PIX 500 铠装式金属封闭开关设备 产品目录》需要特别注意文件名与正文不一致：文件名含 PIX550，但正文真实标题是 [[PIX500]]。PIX500 是 [[PIX]] 家族 500mm 柜宽的小型化 [[空气绝缘开关设备]]，同样面向 12kV、≤1250A、≤31.5kA，但与 [[PIX550]] 的中置式可抽出手车不同，PIX500 采用固定联接主回路、[[HVX]] 固封式断路器和三工位开关，三工位开关具备工作、隔离、接地位置并可在柜前观察。它的叙事更强调替代传统 XGN、减少 30% 配电室土建成本、柜前 1m 维护通道、无 SF6，以及适用于预装式变电站、有轨电车和基础设施场景。

第十八份来源《PIX 户内交流金属封闭开关设备 产品目录 V8》是一个更接近当前产品族总览的修订版。它把 [[PIX]] 从早期 12/24kV 中文目录扩展为 7.2/12/24kV 综合口径，按 GB/T 3906-2020 和 IEC 62271-200:2021 给出参数表：7.2/12kV 内部电弧等级为 AFLR 50kA/1s，24kV 为 AFLR 40kA/1s；12kV 发电机出口断路器柜参数仍可到 6300A/63kA。V8 同时把绿色认证、Green Premium、PCCC、碳足迹、核电、海事、WMTS 电源切换和 [[SmartPIX]] 统一纳入 PIX 叙事。尤其是 Smart PIX 章节，把 PMB/PMB Easy、嵌入式无线测温、断路器特性监测、配柜监测、一键顺控、局放、剩余电寿命、视频、弧光和环境温湿度监测整合到 [[EcoStruxure]] 与千里眼资产顾问的数字化运维链路中。

第十九份来源《WIG 高铁智能开关柜》把知识库从产品目录进一步拉到行业系统集成场景。[[WIG]] 资料围绕 [[数字化变电站]] 展开，强调 IEC 61850、过程层/间隔层/站控层、合并智能单元、保护测控装置、光交换机、网关、辅助监控后台和保护测控后台。其 [[智能监测显示终端]] 把一次回路模拟图、带电显示、断路器机械特性、储能电机、三工位电机、SF6 密度/温度、避雷器、开关柜温度和自动加热除湿控制集中显示，并通过 MODBUS 向监控网络提供遥测/遥信。该资料还明确了多厂家边界：[[成都交大运达]] 偏保护测控，[[常州帕斯菲克]] 偏视窗/后台，[[深圳昇伟电子科技]] 偏智能监测显示终端。需要注意的是，系统图里“Modbus-RTU 转 IEC61580”很可能是 IEC 61850 的笔误，后续工程引用应核对原图纸。

第二十份来源《GHA Gas Insulated Switchgear Presentation Vers 06 English》补充了施耐德另一条 [[气体绝缘开关柜]] 路线。[[GHA]] 被定位为最高 40.5kV、带真空断路器的气体绝缘开关柜，可覆盖单母线和双母线方案；与 [[GMA]] 当前 12/24kV 资料和 [[GMAirSeT]] 环保气体资料相比，GHA 更突出高电压等级、[[BLink]] 无现场气体处理母线连接、[[IDIS]] 气体密度信息系统和 [[ILIS]] 内部故障电弧检测。该资料还补充了外锥/内锥电缆连接、全绝缘母线系统最高 2500A、IAC AFLR 40kA/1s 和抗震选项。由于旧版 PPT 的表格抽取存在碎片化，当前只把能明确抽取的参数写入 wiki，完整选型表仍需后续目录来源复核。

第二十一份来源《GHA Gas-insulated Switchgear Catalog 2018》把上一份旧演示稿中的 [[GHA]] 信息校正为正式目录口径。该目录给出 12/17.5/24/36/38/40.5kV 总额定参数，短时电流 40kA，峰值耐受电流 100kA，母线和支路最高 2500A，母线更高值可按需到 4000A；同时把 IEC 单母线、IEC 双母线、GHA Rail 和 GHA ANSI 分支放在同一产品族内。数字化方面，GHA 被描述为 ready for IoT，并通过 [[EcoStruxure]] ready solutions 连接 Substation Monitoring Device、HMI、Easergy P3/Sepam/MiCOM、VAMP、TH110、CL110、[[IDIS]] 和 [[IVIS]]。需要注意的是，[[BLink]] 峰值电流在旧 PPT 中为 104kA，而 2018 catalog 为 100kA，后续工程引用应优先查具体项目/订货文件。

当前来源之间的主要核对点是可靠性宣传口径：多数资料使用“可靠性提高 1 倍”，但 V3.4 后部页面也出现“可靠性高出 50%”的表达。HVX 说明书中的施耐德公司介绍来自更早时间点，因此企业规模数字与 2020 年样本不同，应按时间差异理解。后续如果再导入更细的二次回路资料、PMB Easy 详细手册或云端运维资料，可以重点比对控制回路、接入数量限制、安装边界和趋势分析输出是否一致。
