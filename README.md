# LigerUI
web前端快速开发后台管理系统的js框架，建立一个后台信息管理系统界面

1、用户管理界面
    
    提供用户列表、添加用户、编辑用户、删除用户等功能，实现列表分页
    
    增加用户数据导出功能
2、ajax请求接口地址封装
    
    通过config文件夹中config.js文件同一封装项目接口地址：
        
        var baseUrl = "http://localhost:8080/BusInfoSystem/";
        var API = {
            //用户列表
            listUser:baseUrl+"user/getListUser",
            deleteUser:baseUrl+"user/deleteUser",
            exportUser:baseUrl+"user/exportUser",
        }
    页面通过<script src="../lib/config/config.js" type="text/javascript"></script>引入配置文件js,
    在对应的ajax url参数位置使用API.listUser等调用相关接口地址
