太原工业学院图书馆自动约坐，每日0点自动约坐下一天，carnumber是学号，labroomld是图书馆馆室的编号，10是六楼男厕所那边的，0-9均有，有问题问吧，懒得看了，seatNum是座位号
提供一个思路，电脑微信使用抓包软件预约图书馆的界面，那个预约是一个网址，用edge游览器获取预约那段时间的请求，然后可以复制成path，有path转Python（具体有点忘记，但是网上一定有教程），学过python的可以使用requests库请求，会返回一个.text报文，然后使用schedule库进每天0点约，最后把代码放到云虚拟机就可以跑起来，最后用Linux的nohup命令把他挂到后台，每天0点自动约座[棒]，只提供思路，我记得网上有类似视频，自己学，也不难
提供一个网站自己看，https://mipweb.tit.edu.cn/schReadingRoomSvg/h5Show/room.html?cardNumber=学号&date=2024-05-13&time=06:30&timeLong=15.5&roomId=10
当然，你也可以使用这个网站直接预约，只需要改学号，日期，预约时长，馆号即可
这个网站使用任意学号进去，修改roomid可以换图书馆馆室，剩下的有问题提，看到会回复
