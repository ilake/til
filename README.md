# Rails
 - Ruby Threads and ActiveRecord Connections
  - http://jakeyesbeck.com/2016/02/14/ruby-threads-and-active-record-connections/
  - http://vigram-software-generals.blogspot.tw/2014/03/ruby-threads-activerecord-too-many.html

#### articles
 - [How DHH Organizes His Rails Controllers](http://jeromedalbert.com/how-dhh-organizes-his-rails-controllers/)


# Javascript
- async/await
  - https://www.twilio.com/blog/2015/10/asyncawait-the-hero-javascript-deserved.html

# React

#### resources
 - https://github.com/bonniee/learning-react-native
 - https://www.youtube.com/playlist?list=PLb0IAmt7-GS0M8Q95RIc2lOM6nc77q1IY
 - [A cartoon intro to redux](https://code-cartoons.com/a-cartoon-intro-to-redux-3afb775501a6#.a9bakoxwt)
 - [2016-03-02 React.js Conf 回顧 @ Reactjs.tw 社群小聚 11](https://docs.google.com/presentation/d/1JEM8YXFM0UUKRL5tyLxCT9tKFgmDDaLPb6UcFetWaBA/edit#slide=id.g11bfd72763_0_104)

#### memo
- require image in react-native
  - http://stackoverflow.com/questions/29308937/trouble-requiring-image-module-in-react-native

#### webpack
- [React with webpack - part 1](http://jslog.com/2014/10/02/react-with-webpack-part-1/)
 - use `render` to replace `renderComponent` http://stackoverflow.com/questions/30698585/react-typeerror-react-rendercomponent-is-not-a-function
- [Getting Started](http://webpack.github.io/docs/tutorials/getting-started/)

# Devops

#### deployment
 - When you have multiple servers for app, workers, search etc... and you have a upgrade like rails 4.1 to rails 4.2. You need to be careful of the different version of these servers. Like Rails 4.2 app, Rails 4.1 worker(app finished deployment first). It may has some problems and you probably need to deploy workers first.
 - Take care of the asset when you use auto-scale, the easist way to avoid any problem, expire everything `Rails.application.config.assets.version = "1.1"`

# Compute sciences
- WebSockets From Scratch
  - https://blog.pusher.com/websockets-from-scratch/

# Issue I met
- [mysqldump special character issue](http://stackoverflow.com/questions/3583691/mysqldump-and-restore-with-special-characters-%C3%B8%C3%A6%C3%A5%C3%98%C3%86%C3%85)

# Tool
- resize icons
  - http://makeappicon.com/

# others guys learning path
- https://www.ptt.cc/bbs/Soft_Job/M.1455389052.A.586.html
- https://www.ptt.cc/bbs/Soft_Job/M.1455442899.A.61B.html
- http://buzzorange.com/techorange/2015/07/28/coder-brand/
- interview
  - https://softnshare.wordpress.com/2016/02/21/%E7%A8%8B%E5%BC%8F%E8%AA%9E%E8%A8%80%E9%9D%A2%E8%A9%A6%E8%80%83%E9%A1%8C%E9%9B%86%E9%8C%A6/
  - system design
    - https://github.com/checkcheckzz/system-design-interview
