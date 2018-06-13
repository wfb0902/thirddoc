# thirddoc
1、直播场次排序  {{vrmu-live}}/live/record/live?pageNo=1&pageSize=10
		开始直播 {{vrmu-live}}/manage/record/start
		结束直播 {{vrmu-live}}/manage/record/end
		增加定时判断直播是否结束，进行判断，防止异常结束直播导致的状态和实际状态差异
2、礼物信息添加字段 
	{{vrmu-live}}/live/room/get-gift    
	{{vrmu-live}}/live/anchor/get-gifts?recordId=6377412323077783556&pageNo=1&pageSize=10&date=2018-3-8
3、用户关注 {{vrmu-user}}/feign/user/follow/isFollow
           {{vrmu-user}}/user/follow/follow
           {{vrmu-user}}/user/follow/cancelFollow
           {{vrmu-user}}/user/follow/taFollow?userId=6347341650485837828&pageNo=1&pageSize=20
           {{vrmu-user}}/user/follow/taFans?userId=6347341650485837828&pageNo=1&pageSize=20
           
4、充值问题定位修复（进一步确认问题，多种方式都存在到账时间过长还是只是个别方式，不同方式服务端走不同外围接口）
5、用户等级，会员充值叠加问题以及有效时间问题，需要一份明确的支持规则才可以评估
6、直播分类，管理后台，涉及接口{{vrmu-live}}/live/record/live?pageNo=1&pageSize=10
7、消息推送，明确是否只是程序启动以后的推送（判断一定逻辑触发自动推送、针对性推送，管理后台是否已经具备能力）
8、机器人功能，1、后台增加机器人管理入口，确认是否存在?
						2、明确加入规则，添加条件
						3、需要模拟那些动作，比如：进入、发言、送礼物、互动、离开房间
9、配合导播台改造，
	正在直播列表，多加一个caster_id字段，字段来源需要明确一下来源接口 {{vrmu-live}}/live/manage/list?pageNo=1&pageSize=10
	还有一个接口，没有明确出来


	
				
