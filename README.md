# Rails
 - Ruby Threads and ActiveRecord Connections
  - http://jakeyesbeck.com/2016/02/14/ruby-threads-and-active-record-connections/
  - http://vigram-software-generals.blogspot.tw/2014/03/ruby-threads-activerecord-too-many.html
 - Time
  - https://github.com/ramhoj/time-zone-article/issues/1
  - http://www.elabs.se/blog/36-working-with-time-zones-in-ruby-on-rails
  - Use `Time.zone.now` or Time.now.in_time_zone("Taipei").to_date
 - Transaction
  - http://markdaggett.com/blog/2011/12/01/transactions-in-rails/
  - raise ActiveRecord::Rollback will invalidate a transaction and reset the database records, won't bubbles up through the application stack

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
- [What is data-react-checksum](http://stackoverflow.com/questions/34311221/what-is-checksum-in-react-and-how-to-use-it)
- [Rendering React Components on the Server](http://www.crmarsh.com/react-ssr/)

#### webpack
- [React with webpack - part 1](http://jslog.com/2014/10/02/react-with-webpack-part-1/)
 - use `render` to replace `renderComponent` http://stackoverflow.com/questions/30698585/react-typeerror-react-rendercomponent-is-not-a-function
- [Getting Started](http://webpack.github.io/docs/tutorials/getting-started/)
- [Howto](https://github.com/petehunt/webpack-howto)
- [Why You Should Try React and Rails Integration Using Webpack](https://www.netguru.co/blog/react-rails-webpack)
- [React on rails](https://github.com/shakacode/react_on_rails/)

# Devops

#### deployment
 - When you have multiple servers for app, workers, search etc... and you have a upgrade like rails 4.1 to rails 4.2. You need to be careful of the different version of these servers. Like Rails 4.2 app, Rails 4.1 worker(app finished deployment first). It may has some problems and you probably need to deploy workers first.
 - Take care of the asset when you use auto-scale, the easist way to avoid any problem, expire everything `Rails.application.config.assets.version = "1.1"`

# Compute sciences
- WebSockets From Scratch
  - https://blog.pusher.com/websockets-from-scratch/
- selec * for update
  - https://gist.github.com/ilake/f163ccf349fdc288e009
  - http://api.rubyonrails.org/classes/ActiveRecord/Locking/Optimistic.html
  - http://stackoverflow.com/questions/21404484/rails-3-how-to-simply-test-pessimistic-locking-on-console
  - [Prevent MySQL deadlocks in your Rails application](https://www.brightbox.com/blog/2014/11/13/preventing-mysql-deadlocks/)
  - [MySQL locking for the busy web developer](https://www.brightbox.com/blog/2013/10/31/on-mysql-locks/)


# Others
 - [The Difference Between ID and Class](https://css-tricks.com/the-difference-between-id-and-class/)

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
