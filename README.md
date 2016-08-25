# Ruby/Rails
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
  - [Transactions are not distributed across database connections](http://api.rubyonrails.org/classes/ActiveRecord/Transactions/ClassMethods.html#module-ActiveRecord::Transactions::ClassMethods-label-Transactions+are+not+distributed+across+database+connections)
  - [nested transaction](http://api.rubyonrails.org/classes/ActiveRecord/Transactions/ClassMethods.html#module-ActiveRecord::Transactions::ClassMethods-label-Nested+transactions)
    -  Active Record emulates nested transactions by using [savepoints](http://dev.mysql.com/doc/refman/5.6/en/savepoint.html) on MySQL and PostgreSQL  
 - Others
  - [config pattern](https://gist.github.com/ilake/fc68aee49aec15a4e2865a635863bb26)
  - [accepts_nested_attributes_for with Has-Many-Through Relations](https://robots.thoughtbot.com/accepts-nested-attributes-for-with-has-many-through)
  - Is Ruby pass-by-reference or pass-by-value?
    - http://robertheaton.com/2014/07/22/is-ruby-pass-by-reference-or-pass-by-value/
    - http://stackoverflow.com/questions/1872110/is-ruby-pass-by-reference-or-by-value
  - rspec controller spec [render_views](https://www.relishapp.com/rspec/rspec-rails/docs/controller-specs/render-views)
  - scan
   - http://stackoverflow.com/questions/1628673/ruby-regex-for-a-split-every-four-characters-not-working
   - https://ruby-doc.org/core-2.2.0/String.html#scan-method

#### articles
 - [How DHH Organizes His Rails Controllers](http://jeromedalbert.com/how-dhh-organizes-his-rails-controllers/)


# Javascript
- async/await
  - https://www.twilio.com/blog/2015/10/asyncawait-the-hero-javascript-deserved.html
- es6 string interpolation
  -  http://stackoverflow.com/questions/21668025/react-jsx-access-props-in-quotes/30061326#30061326
  -  ```{`images/${this.props.image}`}```
- "use strict";
 - http://www.ruanyifeng.com/blog/2013/01/javascript_strict_mode.html
 - https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Strict_mode
 - More serious rules, you could not write javascript whatever you want.
- namespace
 - [pattern example](https://gist.github.com/ilake/ad63c66942c14469291f51d217ae01df)
 - https://addyosmani.com/blog/essential-js-namespacing/
- [Prevent double click script](https://gist.github.com/ilake/b97de5c3235592280a0045b0f48670fd)
- [Window.location](https://developer.mozilla.org/en-US/docs/Web/API/Window/location)
- [String.prototype.replace](https://developer.mozilla.org/zh-TW/docs/Web/JavaScript/Reference/Global_Objects/String/replace)
- Object.assign
 - https://developer.mozilla.org/zh-TW/docs/Web/JavaScript/Reference/Global_Objects/Object/assign
 - [JavaScript 的 Object.assign 陷阱](http://jigsawye.com/2015/10/06/javascript-object-assign/)
- onbeforeunload
 - https://developer.mozilla.org/en-US/docs/Web/API/WindowEventHandlers/onbeforeunload
 - http://stackoverflow.com/questions/30712377/jquery-beforeunload-custom-pop-up-window-for-leaving-a-page
- [How to trigger a click on a link using jQuery](http://stackoverflow.com/questions/5811122/how-to-trigger-a-click-on-a-link-using-jquery)
 - ```$('#test1')[0].click();```
- handle array-like objects
 - http://stackoverflow.com/questions/1424710/why-is-my-join-on-a-javascript-array-failing
 - https://api.jquery.com/jQuery.makeArray/

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

#### others
- [Perform debounce in React.js](http://stackoverflow.com/questions/23123138/perform-debounce-in-react-js/28046731#28046731)
- [React AJAX Best Practices](http://andrewhfarmer.com/react-ajax-best-practices/)
- [React pattern](https://github.com/planningcenter/react-patterns)
- [Container Components](https://medium.com/@learnreact/container-components-c0e67432e005#.4ap4eik7p)
- [Pass value in onClick](http://stackoverflow.com/questions/29810914/react-js-onclick-cant-pass-value-to-method/29810951#29810951)
- [Use setState callback to make sure state be updated](http://stackoverflow.com/a/30783011/609365)
- [React initialize flow diagram](https://hashnode.com/post/why-is-it-a-bad-idea-to-call-setstate-immediately-after-componentdidmount-in-react-cim5vz8kn01flek53aqa22mby)
- [Reactjs Day 5 - Reactjs 大解密](http://ithelp.ithome.com.tw/articles/10156062)
- [controlled & uncontrolled component](https://facebook.github.io/react/docs/forms.html#uncontrolled-components)

# Devops

#### deployment
 - When you have multiple servers for app, workers, search etc... and you have a upgrade like rails 4.1 to rails 4.2. You need to be careful of the different version of these servers. Like Rails 4.2 app, Rails 4.1 worker(app finished deployment first). It may has some problems and you probably need to deploy workers first.
 - Take care of the asset when you use auto-scale, the easist way to avoid any problem, expire everything `Rails.application.config.assets.version = "1.1"`

# Others
 - [The Difference Between ID and Class](https://css-tricks.com/the-difference-between-id-and-class/)
 - [Adjacent sibling selectors, what plus + symbol means in css](https://www.w3.org/TR/CSS2/selector.html#adjacent-selectors)
 - [About line-height](http://muki.tw/tech/css-line-height/)
 - [Ruby 語法放大鏡之「你知道 require 幫你做了什麼事嗎?」](http://kaochenlong.com/2016/05/01/require/)
 - [Ruby class instance variable vs. class variable](http://stackoverflow.com/questions/15773552/ruby-class-instance-variable-vs-class-variable)
 - [How Do I Know Whether My Rails App Is Thread-safe or Not?](https://bearmetal.eu/theden/how-do-i-know-whether-my-rails-app-is-thread-safe-or-not/)
 - CSS display:inline vs inline-block
   - http://stackoverflow.com/questions/8969381/what-is-the-difference-between-display-inline-and-display-inline-block
   - http://stackoverflow.com/questions/9189810/css-display-inline-vs-inline-block
 - code smell
   - https://www.youtube.com/watch?v=PJjHfa5yxlU
   - https://github.com/troessner/reek
 - content too long
  - http://note.tc.edu.tw/714.html
  - `word-wrap: break-word;  overflow: hidden;`
 - mysql explain
  - http://emn178.pixnet.net/blog/post/83011289-mysql-explain---%E6%95%88%E8%83%BD%E5%88%86%E6%9E%90%E8%AA%9E%E5%8F%A5
   - rows lower is better
  - http://fecbob.pixnet.net/blog/post/39084799-mysql-%E4%B8%ADexplain%E7%9A%84%E7%94%A8%E6%B3%95
  - http://database.51cto.com/art/201108/285710_all.htm
   - `type`: from good -> bad. const、eq_reg、ref、range、indexhe then ALL
   - `possible_keys`: when it is empty, it means no possible indexes
   - `key`: what query be used
   - `key_len` lower is better
 - [Why Postgres Won't Always Use an Index](https://robots.thoughtbot.com/why-postgres-wont-always-use-an-index#how-indexes-are-used)
 - WebSockets From Scratch
  - https://blog.pusher.com/websockets-from-scratch/
 - selec * for update
  - https://gist.github.com/ilake/f163ccf349fdc288e009
  - http://api.rubyonrails.org/classes/ActiveRecord/Locking/Optimistic.html
  - http://stackoverflow.com/questions/21404484/rails-3-how-to-simply-test-pessimistic-locking-on-console
  - [Prevent MySQL deadlocks in your Rails application](https://www.brightbox.com/blog/2014/11/13/preventing-mysql-deadlocks/)
  - [MySQL locking for the busy web developer](https://www.brightbox.com/blog/2013/10/31/on-mysql-locks/)
 - [CSS Order Priority](https://hungred.com/useful-information/css-priority-order-tips-tricks/) 
 - [Understanding offsetWidth, clientWidth, scrollWidth and -Height](http://stackoverflow.com/questions/21064101/understanding-offsetwidth-clientwidth-scrollwidth-and-height-respectively)
  - https://developer.mozilla.org/zh-TW/docs/Web/API/Element/scrollWidth
 - css transition
  - https://jsfiddle.net/ilake/jyhLqvuy/17/
  - http://css3.bradshawenterprises.com/accordions/
 - [css text-transform](https://developer.mozilla.org/en-US/docs/Web/CSS/text-transform)
 - HTML property vs attributes
  - http://stackoverflow.com/questions/6003819/properties-and-attributes-in-html
  - http://stackoverflow.com/questions/19246714/html-attributes-vs-properties
  - http://stackoverflow.com/questions/5874652/prop-vs-attr
 - [Determine Whether Two Date Ranges Overlap](http://stackoverflow.com/questions/325933/determine-whether-two-date-ranges-overlap)
 - [vertical-align sample](https://jsfiddle.net/ilake/mzL7arpq/), [vertical-align-sampe-2](https://jsfiddle.net/ilake/7manafyL/)
 - [viewpoint height - Make div 100% height of browser window](http://stackoverflow.com/questions/1575141/make-div-100-height-of-browser-window)
 - [Select where first letter in a range ( PostgreSQL )](http://stackoverflow.com/questions/8085651/select-where-first-letter-in-a-range-postgresql)


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
  - https://www.ptt.cc/bbs/Soft_Job/M.1461981425.A.E04.html
  - system design
    - https://github.com/checkcheckzz/system-design-interview
    - http://www.hiredintech.com/system-design
