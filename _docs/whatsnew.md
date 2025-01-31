---
title: 更新日志
withjs: false
order: 1
category: 帮助与支持
icon: cloud-upload
layout: text-page
---
## 23.05.01
- [dps] 功能更新：选项功能扩展，现在可以支持滚动条和菜单选择了<br>
作为测试，武者的背水效果现在可以选择血量计算了，不是默认叠满<br>
同时在多萝西处加入了“在选项中选择干员”的测试

## 23.04.19-30
- [fix] 优化了抬手计算过程，可以区分召唤物和本体的抬手了
- [fix] 修正陷阱师普攻错误的计算了暴击的问题
- [dps] 调整了Hashtag切换逻辑
- [fix] PR #13 - 修复手机上顶栏的显示 by EE0000
- [fix] #12 - 星熊二模自身加防没有计算
- [fix] 修正一部分额外伤害没有计算增伤倍率的问题：蓝毒、棘刺、奥斯塔、投掷手、特米米、瑕光3、绮良、卡夫卡、乌有
- [fix] 凯尔希3技能的自爆伤害现在在说明栏里列出
- [fix] 修正凯尔希3技能抬手时间为21帧
- [note] 现在暂时无法计算夕第二模组的技力回复效果，需要之后大更新才能加入相关功能
- [update] 更新绿票价值表

## 23.04.10-13
- [update] 伊内丝, 阵法术师/陷阱师/年/刻俄柏/洋灰/摩根模组
- [dps] 暂且优化了NaN的显示……
- [dps] 调整了Logo位置
- [fix] 伊内丝3技能影镖的伤害从偷取0层攻击开始计算（以前多算了200伤害）
- [fix] 重做了白铁的计算逻辑

        2技能：选择“计算召唤物数据”时显示召唤物损血的DPS
        3技能：选择“计算召唤物数据”时，技能/普攻DPS分别代表白铁开启、未开启技能时，铁钳号的伤害
        默认为3s/1次攻击，通过设置攻速可以调整攻击间隔，以计算不同情况下的DPS
- [fix] 决战者未阻挡+无模组时，不回复技力

        这时虽然会计算并显示普攻和技能的DPS，但不代表能开出技能。
        增加了相关提示
- [fix] 玛恩纳第一天赋，现在按实际选择的敌人数量进行判定。敌人数量<3时不强化，>=3时强化（+5%）
- [fix] 冲锋号令类技能的技能输出/时间现在设为0
- [fix] 温蒂3技能水炮伤害，应以本体攻击力计算；计算器屏蔽了勾选召唤物时的计算结果，应该以本体的水炮伤害为准。
- [fix] 修复温蒂模组应该给本体而非召唤物加攻的问题. 鹰语越来越难懂了...
- [fix] 修复芳汀普攻没有计算距离惩罚的问题
- [fix] 修复和弦蓄力攻击错误地乘上了倍率的问题（蓄力应该不加攻）
- [fix] 团辅和敌人数量为空时出错的问题 Issue #5
- [fix][test] Site not correct loading? Issue #10. Still nees testing

## 23.03.20
- [update] 麒麟X夜刀，火龙S黑角，轰击术师/推击手模组，推王、闪灵新模组 <br>
  增加了暂时关闭某个干员的功能。**目前调整中干员：温蒂，白铁** <br>
  更新logo，微调页面布局；预计增加说明和捐助页面 <br>
  微调了时间轴模拟结果的符号规则
- [equip] 模组一览页面，改进了子职业选单
- [mastery] 专精收益图表现在可以在后台设定更多参数了
- [mastery] 更新绿票价值表
- [note] 伊芙利特模组效果，1，3技能以触发1次计算，2技能以平均概率进行模拟（每5/3.33次触发一次），以避免随机模拟导致的结果波动
- [plot] 调整x轴原点位置和字体大小 (Issue #8)
- [fix] 修正夜刀1技能在低攻速下的计算

## 23.03.07
- [fix] 菲亚梅塔2技能阻回暂时订正为84帧固定
- [fix] 修复拜松的第一天赋计算顺序错误的问题，补充2技能防御力计算
- [fix] 夜魔1技能应以攻击力计算治疗量（参见PRTS）（楪筱祈）
- [fix] 耀光第一天赋AOE计算，同时为了避免模组和阻挡选项冲突，暂时去除了模组选项（@Bili 天潭小助，楪筱祈）
- [todo] 已知问题：白铁3技能应享受本体Buff加成
- [todo] 已知问题：推王同分支干员显示undefined乱入错误

## 23.02.17-18
- [fix] 白铁3召唤物的范围伤害(by 糖霜)，召唤物时间轴调整中
- [fix] 仇白2/普攻，勾选距离惩罚时，额外伤害攻击力计算错误(@bili 吃猫咪的香蕉/ 枕头46)
- [fix] 林2技能的攻击准备时间 (@bili reaving)

## 23.02.12-17
- [update] 仇白，铎铃
- [hotfix] 仇白补上天赋倍率(低寄错误)，修正3技能以外的帧数补正数据（普攻和12技能为39帧，3技能基础为40帧）(hxiaiya)
- [hotfix] 2技能的首尾刀额外伤害不享受攻击力加成
- [note] 仇白选项[触发天赋]可以调整第一天赋的覆盖情况，其中：
- 1技能：技能伤害固定触发天赋，结束的aoe伤害勾选时触发，不勾选时不触发
- 2技能：所有伤害固定触发天赋
- 3技能：所有伤害在勾选时触发天赋，不勾选时全不触发。
- 3技能叠层过程中，每一次攻击的帧数均考虑了帧对齐。暂时没有考虑攻速极慢时的特殊情况。
- [note] 距离惩罚：仇白除了2技能攻击伤害以外，所有的技能和额外伤害都不计距离惩罚
- [note] 2技能首刀花费35帧+技能再持续5s，计算器没有考虑攻速变化导致首刀变快的情况。
- [note] 3技能无Buff时，第44次攻击为法伤+不衰减，但是没有攻击力和天赋倍率加成；计算器不计入该次伤害，实际伤害会略高于计算值.(hjhk258)
- [note] 专精收益按2目标计算。
- [update] 微调了边缘计算的逻辑，现在可以对刚好打不出最后一刀的情况进行提示
- [fix] 修正42 3技能的帧数补正数据。黄昏实际动画时间是31帧，抬手10帧，实际攻击间隔补正=1帧(hjhk258)
- [fix] 修正点燃模拟的初始技力多算了1sp的问题（BV1w24y1s7vS）


## 23.01.24-28
- [update] 修正了脱手类技能的DPS计算规则。现在按伤害的实际持续时间计算技能DPS，技能持续时间则用于计算循环周期。(nga Goodox)
- 影响的技能包括：异客3、流明1、火哨1/2、战车1、承曦格雷伊2、波登可2、嘉维尔2 
- [update] 计算过程页面中，增加了说明
- [fix] 寒芒克洛丝的模组选项(bili 凯尔希的脊椎骨)
- [fix] 计算过程页面中，潜能显示错误
- [fix] 修正重岳3技能计算：多目标时只有主目标触发1天赋，其余目标不应触发. 增加了对第一天赋覆盖Debuff的注记
- [fix] 修正重岳2计算：只对主目标计算1天赋和第二段伤害，其余目标不计算

## 23.01.20-21
- [update] 重岳；中坚术师模组；塞雷娅、流明、截云新模组；补充郁金香计算
- [equip] 模组数据表增加了分支职业过滤选项，优化了选择对话框排版
- [mastery] 专精收益图表现在可以在后台设定更多参数了
- [note] 攻回瞬发技能在拥有普攻抬手数据时，按照“取消最后一次普攻后摇”的方式计算。（请参考计算过程）
 目前只在重岳计算中实装了该功能，之后会逐渐补全
- [fix] 风丸1级模组数据错误
- [fix] 重新测量并更新了拳师（斗士）的帧数补正数据，和刻俄柏的抬手时间
- [fix] 火哨1计算错误
- [fix] 赫拉格技能重置普攻设置
- [note] 重岳专精按2目标计算收益
- [fix] 数据源网址调试中 

## 22.12.18-23
- [fix] 焰影苇草2技能火球立即触发时的攻击应为每1.567s触发三次，总共39
- [fix] 宴1级模组计算问题
- [update] 焰影苇草；武者、攻城模组，水月、空弦新模组.
- [update] 更新头像资源，使用Arknights-Bot-Resource库
- [update] 更新抬手时间参考值：空弦，赫拉格
- [dps-todo] 计划加入算法解释板块，对计算时的特殊假设进行详细说明。
- [note] 修改了攻回瞬发技能的抬手计算，具体效果需要观察试验

## 22.12.14
- [mastery] 新增图表：专精提升率对比。可以选择用作基准的练度指标（分母）对比其他练度的提升和损失。
- [mastery] 绿票价值更新，数据格式改为与一图流导出数据兼容.
- [bug] 已知问题：温蒂3技能水炮技能伤害应按照本体的攻击力计算，现在的计算有误，应该直接参照本体的水炮伤害。

## 22.11.10-11
- [fix] 修正了模组覆盖天赋效果的计算
- [fix] 修正了异德2技能抬手时间
- [fix] 修正了异德3技能攻击段数和没有计算普攻的问题.
- [fix] 修正黑第二模组Lv1时错误覆盖天赋的问题

## 22.11.09
- [update] 缄默德克萨斯，白铁
- [equip] 先锋，黑，星熊模组
- [note] 红1、缄默德克萨斯1技能落地有1秒时间，不影响普攻时间。补充了说明
- [note] 砾2技能护盾落地时即衰减10%，实际生效为90%护盾。补充了说明
- [note] 白铁3技能的机器人伤害在召唤物计算选项中，以固定10次攻击计算。
- [dps] 增加了召唤物计算中取本体数值的部分逻辑
- [sim] 增加了对取消普攻前摇的模拟，但暂时没什么卵用
- [sim-fix] 模拟未蓄力技能时，释放技能后应该损失所有剩余的技力。暂时修正。

## 22.10.02
- [update] 医师,安洁夕模组
- [fix] 号角普攻目标数
- [note] 暂时不计算夕2模组的额外技力回复，今后会加入

## 22.09.28
- [update] 海沫，郁金香
- [note] 模组数据暂未更新
- [relic] 收藏品更新水月肉鸽数据，同时增加图片

## 22.09.15-16
- [ranking] DPS表格增加总伤栏
- [update] 罗小黑
- [fix] 修正了切换类技能的描述，改进了潜能选项判定
- [fix] 补充耀光2抬手时间。第18次攻击窗口只有2帧，很可能打不出
- [fix] 年1级模组的加成问题

## 22.09.11-12
- [update] 玛恩纳，但书
- [update] 黑键2，森蚺2，但书，铁卫模组
- [note] 黑键第二天赋，根据设置的敌人数量，判定触发效果。
- [note] 瞬发技能的持续时间为技能动画时间，标注在DPS结果最后一排。表格中的“技能攻击间隔”为无效数值。
- [note] 森蚺/极光阻回时，普攻以180s计算DPS
- [fix] 修正夕的召唤物伤害类型(@树上的燕子)
- [fix] 尝试调整了css版本，需要在移动端进行测试

## 22.08.12-14
- [update] 百炼嘉维尔等
- [update] 改进了条件复选框的文字描述
- [note] 鸿雪的打字机按固定25秒计算，不检测精英化等级；至简的暴击使用期望值进行计算
- [mastery] 图表标题显示额外条件
- [fix] 红豆模组计算错误 @某小达
- [fix] 芙兰卡模组天赋概率 @CelesteTheWitch
- [fix] 温蒂位移伤害计算增伤系数
- [fix] 歌蒂2技能力度
- [fix] 水月模组天赋1目标数
- [fix] 晓歌1天赋增加阻挡判断
- [fix] 异客2天赋
- [note] 由于选择不计算暴击时会出现无意义的计算值，暂时屏蔽了该选项（默认为选中状态）

## 22.07.05-07
- [update] 新干员-多萝西等
- [equip] 更新狙击模组、帕拉斯和麦哲伦的第二模组等计算
- [fix] 山1技能错误的重置普攻的问题

## 22.07.01
- [fix] “修复”了新干员列表出错导致页面无法加载的问题？需要进一步测试
- [fix] 麦哲伦2召唤物攻击类型
- [fix] 黑键2天赋倍率

## 22.06.18
- [mastery] 更新了余下**所有**干员的模组计算，之后逐步修正问题
- [dps] 增加决战者阻回计算逻辑。不选择模组时必须勾选"阻挡"，否则显示为开不出技能的计算结果
- [fix] 修复了召唤物模组加成问题，和凝滞师的技力回复计算

## 22.06.17
- [mastery] 更新模组升级收益计算：艾丽妮，菲亚梅塔，傀儡师
- [note] 目前暂时不能模拟攻回技能吃技力拐的情况
- [note] 专精收益页面只展示本体提升效果，归溟鲨模组对替身输出的提升需要在计算器页面查看。
- [fix] 修正了读取模组数据的问题。除非游戏数据特别指定，模组增加的面板都不会对召唤物起效。
- [fix] 菲亚梅塔2技能现在把2次子爆炸计入总伤（相当于伤害翻倍）
- [fix] 重做了风丸2技能的计算。勾选【替身】/【召唤物】时分别显示替身和2技能纸偶的落地伤害，不在本体计算中显示。
- [fix] 修正了yj修复后的异客1技能计算
- [fix] 修正了车尔尼的DPS，并显示反击伤害（不计入dps）
- [fix] 修复了专精收益计算器选择链术师以后换人，目标数出错的问题

## 22.06.15 续
- [mastery] 更新模组升级收益计算：群愈师，处决者，链术师，剑豪（除陈），冲锋手
- [mastery] 优化显示效果
- [relic] 更新收藏品
- [fix] 修复了干员选单的误报

## 22.06.15 模组升级重大更新
- [dps] 增加对模组升级的计算支持；各个干员的具体计算结果在今后分批更新。
如果计算时出现**“暂未更新2-3级模组计算”**的提示，说明这个干员模组升级的效果没有被现版本计算器计入dps，结果无效。
这些干员只有1级模组的计算结果是有效的。
- [dps] 增加支持选择多个触发条件。具体涉及的干员在今后分批更新。
鼠标移到触发条件的选项上，可以显示对应的原版天赋介绍（只作为提示作用，不显示被模组修改过的天赋内容）
- [equip] 模组一览页面可以显示各个等级模组的具体数值。请使用页面搜索进行搜寻，或者点击表头可以进行排序。
- [mastery] 增加了部分干员模组升级收益的计算，具体计算结果在今后分批更新
没有更新的干员会显示“模组升级收益暂未更新”，敬请期待。
- [mastery] 增加了模组升级材料的绿票和龙门币计算
- [mastery] 初步改进了图表配色
- [update] 黑键等
- [update] 更新模组升级收益计算：召唤师，秘术师，教官（除诗怀雅），神射手
- [note] 短时间内不会更新诗怀雅的计算_(:з」∠)_
- [update] 新干员动画数据和头像
- [fix] 对角色等级、技能等级等选择范围做了一定限制，应该能减少一部分不合理选项
- [fix] 修改了页面显示问题
- [fix] 批脸陈换回精一头像_(:з」∠)_

## 22.06.05-
- [beta] 增加模组升级材料消耗测试，正式结果以游戏实装为准

## 22.05.30-06.01
- [fix] 洛洛2技能-叠层倍率
- [fix] 异客1技能-攻击倍率和目标数
- [fix] 瑕光2技能-动画时间和攻击次数

## 22.05.22-23
- [update] 埃拉托
- [ranking] 更新dps统计表，增加模组
- [fix] 叠层技能逻辑错误
- [fix] 修正暴行和九色鹿潜能
- [fix] 异客3技能持续现在按1.2s计算
- [note] 全部改为国内js/css源

## 22.05.04-13
- [update] 优化DPS页面移动端排版
- [update] 专精计算器增加显示专精的提升百分比（不包含模组和潜能）
- [fix] 归溟鲨替身按每秒计算秒伤
- [fix] 艾丽妮技能都是必定穿防
- [fix] 流明1技能计算距离惩罚
- [update] 归溟幽灵鲨等
- [update] 载入和页面逻辑改进，模组页面优化
- [update] 增加了载入进度条
- [update] 新选项-永续技能按180s计算
- [fix] 先计算数值无视防御，再计算百分比无视防御
- [note] 目前计算器不考虑因为攻速变化导致的技能动画时间变化

## 22.04.26
- [fix] 重做了赫默的计算
- [fix] 令3技能小龙攻击类型错误

## 22.04.21
- [fix] 号角3技能损血计算
- [update] 增加了新干员的新版动画数据
- [update] 更新了绿票价值表
- [update] 模组一览增加了子职业图标

## 22.04.17-v2
- [update] 模组数据
- [update] 优化了计算器版本显示
- [equip] 优化了模组列表页，现在可以显示小作文了
- [fix] 褐果1技能应为手动穿插
- [fix] 删除了模组泄漏数据

## 22.04.17
- [update] 号角
- [todo] 模组尚未更新
- [update] 增加了菲亚梅塔动画数据、帧数补正和2技能时间轴模拟
- [update] 干员选单新增【同分支干员】分类
- [update] 增加了过载模式的计算逻辑。计算过程会分别展示普攻、技能前半和过载阶段的输出数据
- [update] 新选项-近战攻击。勾选时表示（号角）使用近战，不造成范围伤害
- [update] 新选项-过载立即结束。勾选时表示过载启动时立即手动结束技能（以避免或产生副作用）
- [update] 修改了以下计算过程的文字描述：**重置普攻、帧数补正、抬手时间默认值、元素治疗**
- [note] 驭械术师的帧数延迟不是因为攻击间隔>动画帧数导致的，而是和浮游炮有关。计算器现在的设定是所有的驭械术师都加上了1帧延迟
- [note] 洛洛的过载期间浮游炮倍率以1.1起算，虽然实战很难打出这样的效果
- [update] 蜜莓1技能现在计算3秒内的总元素回复量
- [fix] 风丸的额外伤害在计算过程中的显示错误（DPS没出错）
- [fix] 删除了错误的动画数据

## 22.04.06
- [fix] 更新群法的帧数补正数据。无模组的群法dps进一步降低了......

## 22.03.20
- [fix] 菲雅3掉血向上取整
- [fix] 一部分干员额外伤害没有乘算damage\_scale
- [fix] DPS数据表格 - 保留3位小数。仍然不推荐查这个表。结果以计算器页面为准

## 22.03.16-17
- [update] 菲雅梅塔等干员，炮手等模组数据
- [note] 菲雅的掉血为每0.1s流失0.5%当前HP（向上取整），计算器给出最大的（满血时）生命流失的hps。
- [note] 菲雅2技能列出子爆炸伤害，不计算期望命中段数
- [note] 优化了对傀儡师属性计算的描述，现在替身的技能dps被设为0了
- [note] 风丸的2技能召唤物属性等于满信赖的本体属性，在信赖不满时攻击力会有区别。为了简化，计算器统一按本体属性计算。
         2技能召唤物落地伤害在本体结果中显示；阵亡后替身的落地伤害需要勾选【傀儡师替身】计算
- [issue] 已知问题：新干员的动画数据无法导入，以后再尝试；增加了对暂无动画数据的角色的判断
- [update] 补充莫斯提马3抬手数据

## 22.02.16-17
- [fix] 修正了澄闪3的前摇，实战帧数会在38-40帧之间浮动，无攻速加成时也可能打出24次攻击
- [bugfix] 澄闪普攻不会爆炸，之前计算有误
- [update] 澄闪
- [note] 澄闪的爆炸概率是每次攻击1.5%递增，爆炸攻击次数的期望是9.91。计算器按10%概率计算
- [note] 驭械术师的普攻、技能均按照**新目标逐渐叠层**计算。如果技能开启时就是满层，实际dps会比计算器显示的值更高（达到理论上限）

但是澄闪2是以**最高倍率**计算（假设永续技能+攻击无限血量木桩，一直都是最高倍率）

## 22.01.29-02.02
- [bug] 已知问题：炎客模组属性显示错误（实际为常态+4攻速/触发+30攻速，计算没问题）
- [fix] 令3可重置普攻
- [bugfix] 夜半专精收益以token计算
- [bugfix] 老鲤2/3技能伤害类型（应为物理）

## 22.01.26
- [update] 令/老鲤
- [note] 令3技能的地板伤害是按照令的面板计算，所以去掉“计算召唤物数据”选项才能显示这部分伤害
- [update] 剑圣、行商、令模组
- [bugfix] 森蚺1/老鲤2的被动效果对普攻也生效
- [bugfix] 麦哲伦3/令3攻击目标数量

## 22.01.10-11
- [bugfix] 收藏品列表parse blackboard没有显示所有词条
- [update] 九色鹿
- [update] 新增【专有名词】术语速查表，【集成战略】收藏品列表
- [update] 侧边栏内容重新分组，增加更新日志按钮
- [update] 【干员属性】页面改为头像，之后会重新排版

## 22.01.05-07
- [update] 暮落
- [bugfix] 暮落1技能攻击间隔为乘算
- [fix] 干员列表增加了区分肉鸽干员的前缀提示
- [mastery] 专精图表增加了对特殊计算条件的说明

## 21.12.30
- [fix] 修正灵知3/耶拉2帧数补正数据

## 21.12.22
- [update] 灵知等
- [update] 模组更新：剑豪，冲锋手
- [update] 灵知3/薄绿2：终结伤害动画时间计入技能用时
- [sim] 增加了对蓄力技能的模拟支持
- [bugfix] 稀音2的伤害类型（应为物理），模组不影响召唤物面板
- [site] 恢复使用jsdelivr CDN，但是提供了本地CDN备选

## 21.11.08
- [bugfix] 耀骑士临光的1天赋落地伤害，2技能落地时间
- [bugfix] 桑葚1天赋选项

## 21.11.04
- [update] 耀骑士临光等
- [update] 改进了链法的计算逻辑。在专精计算器中，链法的收益以2目标计算
- [equip] 更新模组；优化了模组页面的默认排序

## 21.10.17-19
- [update] 远牙等
- [bugfix] 远牙2-3技能重置普攻

## 21.10.08
- [mastery] 新图表引擎测试

## 21.09.22
- [bugfix] 修正了教官模组计算问题。阻挡时倍率不应生效
- [bugfix] 修正了调香师模组的目标数问题

## 21.09.17
- [update] 琴柳等
- [update] 优化了技能、模组信息显示，现在可以正确显示参数和术语了
- [update] 优化了选人菜单
- [todo] 新材料绿票价值为暂定。下月更新
- [bugfix] 列出了模组增加的三围以外的属性（例如夜莺的法抗，杜宾攻速），并且代入计算

## 21.09.06
- [mastery] 专精收益计算器增加计算模组的等效绿票（模组数据块目前按200绿票计）

## 21.08.18
- [plot] 增加技能总伤害曲线；改善了图表切换的表现；x轴增加参数说明

## 21.08.10
- [mastery] 专精收益计算器，图表功能更新模组
- [bugfix] 专精收益计算器和地图显示功能小修，更新数据

## 21.08.05
- [update] 水陈等，新子职业-解放者、收割者
- [update] 新干员皮肤头像和动作数据
- [note] 陈3技能游戏中存在Bug，不受攻速影响；dps计算器仍按正常逻辑计算
- [dps] 增加了[模组]信息页面以及dps计算器相关选项。
- [dps] 增加了弹药类/蓄力类技能算法
- [bugfix] 锡兰的攻击力天赋
- [hotfix] 龙舌兰1技能蓄力时间
- [hotfix] 水陈1天赋显示概率
- [bugfix] 煌3技能的额外伤害攻击力计算错误(b站 朽木有余)
- [dps] 恢复考虑技能取消攻击间隔（例如水陈1，柏喙2）。暂时没有计算抬手时间

## 21.07.30
- 此版本为模组更新前的备份Tag版本，用于对比
- [mastery] 新增了官方子职业名称分类

## 21.07.27
- [mastery] 新增了对子职业的分析测试
- [dps] 帧数计算部分调整中

## 21.07.22
- [dps] 增加了帧数计算的测试。由于结果误差较大，不代入后续计算。只作为参考
- [dps] 修改了迷迭香3技能的计算方式。现在可以对单目标计算重叠伤害，增加了是否计算战术装置减防的开关
- [bugfix] 专精收益和图表页面载入动作数据
- [bugfix] 敌人数值和团辅现在能正确的输入小数了

## 21.07.18-19
- [dps] 更新动画帧数查看功能（测试）
- [dps] 修改了攻回瞬发技能的计算逻辑，现在按完整循环来计算（不使用技能取消普攻攻击间隔）. 受影响的有例如柏喙2技能 -- 21.08.05 已回卷
- [dps] 原有的“触发天赋”选项，现在能够显示具体触发的哪个天赋的提示（例如“触发 - 空射专精”）
- [bugfix] 梅尔2技能。现在不勾选“计算召唤物数据”可以得到正确的结果，勾选时会有（应该去掉该选项）的额外提示
- [bugfix] 柏喙1技能攻击目标
- [bugfix] 远山的帧数补正。今后会进行公式化处理，不再一一更新。
- [bugfix] 暴行的3-6潜能无法计算。现在会默认选择2潜能进行计算，选择3-6潜能还是会报错，但是在下侧说明里有相应的提示。

## 21.07.01-02
- [update] 帕拉斯
- [update] 更新了支援近卫的特性
- 专精收益计算器：增加了json输出和hashtag处理
- dps图表：增加了json输出，改用新版选人画面

## 21.06.16
- 将标题图修改为cdn获取（没有cdn寸步难行……）

## 21.06.07
- [update] 卡涅利安完成计算。增加了贝娜替身的计算
- [update] 增加了新干员头像，和凯尔希/卡涅的抬手数据
- [dps] 使用逐次计算的方法重写了可变攻击力计算
- [dps] ~~增加了单次攻击的dps计算，方便与手算结果比对（直接用单次伤害/攻击间隔，不考虑暴击和技能期间的攻击力变化）~~ 误差太大，取消了
- [fix] 修正爱丽丝的蓄力计算
- [fix] 地图信息页面改为使用CDN数据加速
- [todo] 更新了对于帧数补偿的描述，今后会逐步更新这部分算法。
- [todo] 目前暂时取消了所有抬手时间的缩放计算，这会导致一些计算（例如熊猫）出问题，但是会有更准确的解决方案

## 21.06.01
- [update] 卡涅利安等
- [dps] 新版选人菜单测试
- [dps] 切换类技能（银灰2，山2）统一按永续类计算
- [mastery] 专精收益计算器改版。全面修改为无需后台工作的绿票算法
- [mastery] 去除了部分图表，增加了精二材料计算和收益饼图
- [fix] 修正异客3持续时间，凯尔希3增加误差说明
- [fix] 修正因陀罗1，贝娜1的无视防御计算
- [fix] 修正爱丽丝/守林人/W的炸弹计算，现在炸弹的数量不会超过设定的敌人数量

## 21.05.02 2周年版本
- [update] 浊心斯卡蒂等
- [mastery] 专精收益计算器可以对特定技能按照召唤物计算收益
- [bugfix] 修正了召唤物攻击间隔的计算，现在可以正确计算召唤物的攻速团辅了
- [dps] 修改了攻击类型判断逻辑，现在更乱了
- [dps] 增加了歌辅增加攻击力数值的note

## 21.04.15
- [update] 异客等

## 21.04.11
- [bugfix] 修正了惊蛰的弹射公式。以前将倍率计算了两次。现在改为正确的连续乘算

## 21.03.18
- [bugfix] 修正战车2技能帧数

## 21.03.09
- [dps] 新干员-Ash等

## 21.02.22-27
- [dps] 增加了攻击间隔显示和PRTS链接。顶部增加“问题反馈”信息
- 放出了原本的家具和dps表格页面
- [dpsv2] 调整排版。仍存在很多问题

## 21.02.06
- [update] 夕等
- [dpsv2] 暂时隐藏v2入口。坑填好再补上
- [bugfix] 推王2技能目标数
- [bug] 已知问题：夕1技能召唤物dps不准确。以2/3技能的为准
- [bugfix] 炎狱炎熔1技能对单体攻击次数

## 21.01.19
- [update] 图耶

## 21.01.07-13
- [update] 增加迷迭香1，爱丽丝2动画时间
- [bugfix] 修正了42无视法抗的计算方式
- [bugfix] 修正了黑3技能的攻击间隔

## 21.01.06
- [update] 空弦等
- [dps] 伴随空弦的实装，增加了对一部分攻回技能的模拟计算，同时修正了模拟时对sp上限的限制条件和sp恢复超过上限时的提示。
    
    重写了攻回技能的sp计算逻辑，增加了在空弦/陈天赋加成下的模拟计算。这只是v1版本的临时解决方案，在v2中将给出更通用的攻回技能模拟机制。
    
    在一部分干员上增加了[呵斥][兰登战术]辅助选项，该选项独立于团辅选项生效
- [todo] v2版本暂未更新

## 20.12.23-27
- [bugfix-v1] 山暴击率
- [dpsv2] 修正js依赖问题，干员头像升级(由PRTS Wiki提供数据支持)，现在手机可以看到结果了。
- [customdata] 添加近卫阿米娅和42的抬手数据
- [npm] npm包更新至对应版本

## 20.12.20
- [temp] 补充新干员临时头像
- [bugfix-v1] 山2技能目标数

## 20.12.17
- [update] 更新：山等
- [dps] 优化了切换类技能的循环计算方式

## 20.12.16
- [dpsv2] v2测试版页面开放
- [issue] **已知问题：原版计算中，多数额外伤害没有计算damage_scale**
- [gamedata] 更新游戏数据，增加了角色头像

## 20.12.02
- [dpsv2] 阶段性进展
- [bugfix] 灼地等每秒计算的技能在叠加攻速团辅时应该仍然以1秒间隔计算

## 20.11.19
- [bugfix] 古米2技能时间（实际为40s）增加了对暴击不生效的提示
- [dps] 瞬发技能的dps解除隐藏
- [bugfix] 尝试修改版本更新逻辑

## 20.11.15
- [bugfix] 锡兰1，阿2天赋
- [bugfix] 古米2技能时间

## 20.11.02
- [update] 阿米娅（近卫 ver）
- [plot] 增加了坐标轴标题
- [bugfix] 絮雨talent_scale
- [bugfix] 新材料名称修正

## 20.11.01
- [update] 迷迭香等
- [bugfix] 移除古米/泥岩的摸摸鱼时间
- [todo] 暂未更新阿米娅

## 20.10.16
- [bugfix] 夜魔1技能目标数

## 20.10.15
- [update] 瑕光等
- [bugfix] 龟龟2技能开启时不攻击

## 20.09.24
- [update] 史尔特尔等。开始开发新版引擎

## 20.08.25-30
- [update] 森蚺等，30日更新集成战略干员。增加了对无视魔抗的计算

## 20.08.17
- [bugfix] 绝影攻击间隔错误
- [bugfix] 跃浪击/砾技能时间错误

## 20.08.12
- [update] 棘刺等
- [update] 增加了对毒伤和暖机的说明。棘刺和小羊1的暖机使用统一的选项控制  

## 20.07.30
- [update] 稀音等
- [bugfix] 判断了白金天赋的上下限，以及一般攻速的上下限。攻速达到上下限时会有额外提示。
- [bugfix] 优化了召唤物攻击类型的判定，同时可以大致正确的显示召唤角色的专精收益了。
- [bugfix] 模拟轴计算时判断了充能上限。
- [info] 优化了提示性文字
- [info] 增加了白雪丢失伤害的Bug提示
- [info] 增加了空/铃兰第一秒无治疗效果的Bug提示
- [log] 调换了详细信息中，技能和普攻的顺序。现在技能在前

## 20.07.17 
- 更新了卡达等人的帧数补正数据

## 20.07.14
- 改进了缓存设置

## 20.07.09
- [update] 铃兰等
- [ui] 增加了浏览器兼容性问题提示
- [BUG] 已知问题: Safari浏览器下拉菜单无法正常显示。尝试修复无果

## 20.07.08
- 修改了大量UI效果和计算过程描述排版
- 较小的json不使用cdn处理，增加灵活性

## 20.06.27
- 增加了提示文字，修改了详细信息的格式

## 20.06.24
- 建立此文档。逐步补充以前的更新记录
- [ui] 完善UI元素（logo、链接等）

## 20.06.23
- [weavingGain]  调整了**OGCD技能（例如陨星2）**的周期时间，以**（完整普攻时间+技能动画时间）**计算。实战如将技能穿插在普攻中，则可以略微加速技能周期，提高dps。dps计算结果中没有计入这部分收益，但是在下方给出了穿插收益的估算
- [grad] 重新计算了**煌3、傀影2**的每击伤害。旧算法在抛光时会少算一部分伤害
- 调整了一部分用语，减少歧义

## 20.06.18
- [update] 新干员：早露等
- [edef_pene] 增加了无视护甲机制的计算，现在可以正确计算**送葬人**和**早露**的伤害了
- 调整了一部分用语

## 20.06.16
- [bugfix] 订正了瞬发技能时间的判断错误

## 20.06.02
- [update] 新干员：石棉等

## 20.05.31
- [mastery] 增加了**推荐等级**功能，会根据专精收益和升级收益的比例计算一个推荐的专精等级
- [bugfix] 修正了初始sp的一个错误

## 20.05.29
- [mastery] 增加了升级收益曲线图（在最下面）

## 20.05.28
- [bugfix] 修正了暴击时未计算团辅的bug
- [bugfix] 修正了召唤物的攻速

## 20.05.22
- [bugfix] 修正了刻刀天赋。现在每次2连击会判定2次天赋

## 20.05.18
- [bugfix] 修正了末药的动作时间

## 20.05.16
- [sim] 重写了模拟部分，现在可以估算瞬发技能的时间轴，得到更准确的结果

## 20.05.14
- [bugfix] 修正了之前煌3导致的其他群卫目标数错误

## 20.05.13
- [plot] 完成了**DPS图表**功能，碉堡了！

## 20.05.05
- [bugfix] 修正了煌3的目标数
- 增加了W的动作时间数据

## 20.05.01
- [update] 新干员：W等
- [bugfix] 增加了召唤物的攻速计算
- [plot] 施工中

## 20.04.28
- [ui] 改变左侧元素排序，增加了链接
- [plot] 开坑

## 20.04.22
- [update] 新干员：傀影等

之前的不写了。咕咕咕
