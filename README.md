# Ruby/Rails
 - Ruby Threads and ActiveRecord Connections
  - http://jakeyesbeck.com/2016/02/14/ruby-threads-and-active-record-connections/
  - http://vigram-software-generals.blogspot.tw/2014/03/ruby-threads-activerecord-too-many.html
  - [Ruby Concurrency and Parallelism: A Practical Tutorial](https://www.toptal.com/ruby/ruby-concurrency-and-parallelism-a-practical-primer)
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
  - [Checking assoication exists](http://stackoverflow.com/a/6261813/609365)
  - [filter attributes changes](http://apidock.com/rails/ActiveModel/Dirty/attributes_changed_by_setter)
    - `attributes_changed_by_setter.except!(:foo, :bar)`
  - [glob a directory in Ruby but exclude certain directories?](http://stackoverflow.com/questions/4505566/is-there-a-way-to-glob-a-directory-in-ruby-but-exclude-certain-directories)
    - [WARNING!!!](http://stackoverflow.com/questions/4505566/is-there-a-way-to-glob-a-directory-in-ruby-but-exclude-certain-directories#comment62698604_27707682)
   - [Using heredoc for prettier Ruby code](https://makandracards.com/makandra/1675-using-heredoc-for-prettier-ruby-code)
 - SSL Stuffs
   - [What does force_ssl do in Rails?](http://stackoverflow.com/questions/15676596/what-does-force-ssl-do-in-rails)
   - [config.force_ssl is different than controller force_ssl](http://www.eq8.eu/blogs/14-config-force_ssl-is-different-than-controller-force_ssl)
   - [Dangers of Session Hijacking](http://railscasts.com/episodes/356-dangers-of-session-hijacking?autoplay=true)
   - [How can I make cookies secure (https-only) by default in rails?](http://stackoverflow.com/questions/3773605/how-can-i-make-cookies-secure-https-only-by-default-in-rails)
 - concurrency, parallal
   - [Ruby SSE Server 動手做](https://tonytonyjan.net/2015/11/05/concurrent-ruby/)
   - [Expeditor provides asynchronous execution and fault tolerance for microservices](https://github.com/cookpad/expeditor)
   - [利用 Celluloid Future 在 Ruby 中平行化處理 I/O](http://blog.brucehsu.org/posts/2017/02/04/utilize-celluloid-future-for-parallel-io-tasks/)
     - https://www.facebook.com/groups/208890269174940/permalink/1348477431882879/
     - [I/O Model](https://wirelessr.gitbooks.io/working-life/content/io_model.html)
     - [Ruby concurrency explained](http://merbist.com/2011/02/22/concurrency-in-ruby-explained/)
     - [What is the difference between a thread and a fiber?](http://stackoverflow.com/questions/796217/what-is-the-difference-between-a-thread-and-a-fiber)
     - [Is non-blocking I/O really faster than multi-threaded blocking I/O? How?](http://stackoverflow.com/questions/8546273/is-non-blocking-i-o-really-faster-than-multi-threaded-blocking-i-o-how)
     - [Scalable Event Multiplexing: epoll vs. kqueue]
  - Actor
     - [基於 Actor 模式並發的介紹 (Ruby)](https://www.oschina.net/translate/ruby-gentle-introduction-to-actor-based-concurrency)
     - [A gentle introduction to actor-based concurrency](http://practicingruby.com/articles/gentle-intro-to-actor-based-concurrency)

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
- [What does setTimeout with a 0ms delay do?](https://www.quora.com/What-does-setTimeout-with-a-0ms-delay-do)
 - Let some function be executed immediately right after after the currrent function
- [JavaScript Promise 實作理解筆記](http://opass.logdown.com/posts/296834-javascript-promise-for-see-notes)
- [npm install --save-dev vs npm --save](http://stackoverflow.com/questions/19578796/what-is-the-save-option-for-npm-install)
 - [What does -save-dev mean in npm install --save-dev](http://stackoverflow.com/questions/19223051/grunt-js-what-does-save-dev-mean-in-npm-install-grunt-save-dev)
- What is yarn
 - [取代 npm 的新利器 Yarn](https://medium.com/@jackypan1989/%E5%8F%96%E4%BB%A3-npm-%E7%9A%84%E6%96%B0%E5%88%A9%E5%99%A8-yarn-7d97f2f409b9)
 - [[譯] Yarn - Javascript 新一代套件管理](http://andyyou.github.io/2016/10/12/new-package-manager-javascript-yarn/)
 - [Migrating from npm](https://yarnpkg.com/lang/en/docs/migrating-from-npm/)
 - [webpack](https://webpack.js.org/guides/get-started/)
   - [webpack concept](https://webpack.js.org/concepts/)
   - [webpack configuration](https://webpack.js.org/configuration/)
     - [What does “publicPath” in webpack do?](http://stackoverflow.com/questions/28846814/what-does-publicpath-in-webpack-do)
     - What is loader for?
       - webpack僅能處理Javascript所以需要一些Loader來幫忙。例如,處理CSS檔案，我們需要使用style-loader。
   - [如何使用 Webpack 模組整合工具](https://rhadow.github.io/2015/03/23/webpackIntro/)
   - [WEBPACK入門教學筆記](http://blog.kkbruce.net/2015/10/webpack.html#.WPdwIlOGNE5)
   - [babel-loader jsx SyntaxError: Unexpected token](http://stackoverflow.com/questions/33460420/babel-loader-jsx-syntaxerror-unexpected-token)
    - even react need babel support
    - [babel presets](https://babeljs.io/docs/plugins/#presets)
    - styling
      - [webpack styling](https://medium.com/statuscode/introducing-webpacker-7136d66cddfb#3181)
    - [Using Webpack in Rails with the Webpacker Gem Video](https://gorails.com/episodes/using-webpack-in-rails-with-webpacker-gem?autoplay=1)
 - import, export
  - [Why es6 react component works only with “export default”?](http://stackoverflow.com/questions/31852933/why-es6-react-component-works-only-with-export-default)
  - [ES6 - Convert from 'require' to 'import'](http://stackoverflow.com/questions/30898686/es6-convert-from-require-to-import)
  - [ES6: `import * as React` vs `import React`](https://discuss.reactjs.org/t/es6-import-as-react-vs-import-react/360/3)

# React

#### resources
 - https://github.com/bonniee/learning-react-native
 - https://www.youtube.com/playlist?list=PLb0IAmt7-GS0M8Q95RIc2lOM6nc77q1IY
 - [A cartoon intro to redux](https://code-cartoons.com/a-cartoon-intro-to-redux-3afb775501a6#.a9bakoxwt)
 - [2016-03-02 React.js Conf 回顧 @ Reactjs.tw 社群小聚 11](https://docs.google.com/presentation/d/1JEM8YXFM0UUKRL5tyLxCT9tKFgmDDaLPb6UcFetWaBA/edit#slide=id.g11bfd72763_0_104)

#### react native
  - http://school.shoutem.com/
    - [React Native 101: Build your first mobile app](http://school.shoutem.com/lectures/react-native-101-build-first-mobile-app/)
    - [Build an Imgur App with React Native and MobX](http://school.shoutem.com/lectures/build-simple-imgur-client-react-native/)
      - https://github.com/Swizec/ImgurApp
#### memo
- require image in react-native
  - http://stackoverflow.com/questions/29308937/trouble-requiring-image-module-in-react-native
- [What is data-react-checksum](http://stackoverflow.com/questions/34311221/what-is-checksum-in-react-and-how-to-use-it)
- [Rendering React Components on the Server](http://www.crmarsh.com/react-ssr/)

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
- ref
  - [[Reactjs] 關於 Refs](http://andyyou.logdown.com/posts/179646-reactjs-regarding-the-refs)
    - 不要在 render() 方法裡面使用 this.refs 或者當任何元件的 render() 正在運行的時候。
  - [Using ref Attribute](https://www.reactenlightenment.com/basic-react-components/6.9.html)
- Higher order component
  - [Mixins Considered Harmful](https://facebook.github.io/react/blog/2016/07/13/mixins-considered-harmful.html)
  - [THE POWER OF THE HIGHER ORDER](http://blog.scottlogic.com/2016/09/20/the-power-of-the-higher-order.html)
  - [React Higher Order Components in depth](https://medium.com/@franleplant/react-higher-order-components-in-depth-cf9032ee6c3e#.qo9gmckay)
  - [Higher-Order Components](https://facebook.github.io/react/docs/higher-order-components.html)
  - [Mixins Are Dead. Long Live Composition](https://medium.com/@dan_abramov/mixins-are-dead-long-live-higher-order-components-94a0d2f9e750#.hfk3cfnag)
  - [React進階——使用高階組件（Higher-order Components）優化你的代碼](https://segmentfault.com/a/1190000004598113)
- [ES6篇 - let與const](http://ithelp.ithome.com.tw/articles/10185142)
- [ES6篇: Module System(模組系統)](http://ithelp.ithome.com.tw/articles/10185692)
- [ES6篇 - Class(類別)](http://ithelp.ithome.com.tw/articles/10185583)
- [Destructuring Assignment(解構賦值)](http://ithelp.ithome.com.tw/articles/10185430)

# Devops

#### deployment
 - When you have multiple servers for app, workers, search etc... and you have a upgrade like rails 4.1 to rails 4.2. You need to be careful of the different version of these servers. Like Rails 4.2 app, Rails 4.1 worker(app finished deployment first). It may has some problems and you probably need to deploy workers first.
 - Take care of the asset when you use auto-scale, the easist way to avoid any problem, expire everything `Rails.application.config.assets.version = "1.1"`
 
# DB related
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
   - [Why does PostgreSQL perform sequential scan on indexed column?](http://stackoverflow.com/questions/5203755/why-does-postgresql-perform-sequential-scan-on-indexed-column)
 - selec * for update
  - https://gist.github.com/ilake/f163ccf349fdc288e009
  - http://api.rubyonrails.org/classes/ActiveRecord/Locking/Optimistic.html
  - http://stackoverflow.com/questions/21404484/rails-3-how-to-simply-test-pessimistic-locking-on-console
  - [Prevent MySQL deadlocks in your Rails application](https://www.brightbox.com/blog/2014/11/13/preventing-mysql-deadlocks/)
  - [MySQL locking for the busy web developer](https://www.brightbox.com/blog/2013/10/31/on-mysql-locks/)
 - [Select where first letter in a range ( PostgreSQL )](http://stackoverflow.com/questions/8085651/select-where-first-letter-in-a-range-postgresql)
 - [Determine Whether Two Date Ranges Overlap](http://stackoverflow.com/questions/325933/determine-whether-two-date-ranges-overlap)
 - [GROUP BY multiple columns using MySQL](http://stackoverflow.com/questions/1841426/is-it-possible-to-group-by-multiple-columns-using-mysql)
 - postgresql time/date
   - [compare only time/date part of dateime](http://stackoverflow.com/questions/10298538/handling-time-using-postgresql)
   - [8 PostgreSQL Date and Time Function Examples](http://www.thegeekstuff.com/2010/07/8-postgresql-date-and-time-function-examples/)
     - now(), now()::date, now()::time, date_part(), age(), extract(), date_trunc(), to_char(), to_timestamp()
   - [4 Tips for Working with Dates in PostgreSQL](http://blog.trackets.com/2013/08/26/4-tips-for-working-with-dates-in-postgresql.html)
     - now, extract, interval, clock_timestamp
   - [9.9. Date/Time Functions and Operators](https://www.postgresql.org/docs/9.2/static/functions-datetime.html)
 - PostgreSQL search
   - [Pattern matching with LIKE, SIMILAR TO or regular expressions in PostgreSQL](http://dba.stackexchange.com/a/10696/36173)
   - [PostgreSQL query performance variations](http://stackoverflow.com/a/13452528/609365)
   - [Difference between GiST and GIN index](http://stackoverflow.com/a/28976555/609365)
 - [Using COALESCE to handle NULL values in PostgreSQL](http://stackoverflow.com/questions/27479180/using-coalesce-to-handle-null-values-in-postgresql)
   - COALESCE, NULLIF
 - [Difference between LIKE and ~ in Postgres](http://stackoverflow.com/questions/12452395/difference-between-like-and-in-postgres/12459689#12459689)
 - [How to Create Postgres Indexes Concurrently in ActiveRecord Migrations](https://robots.thoughtbot.com/how-to-create-postgres-indexes-concurrently-in)
 - Postgresql tr_gram, Trgrams
   - [Faster PostgreSQL Searches with Trigrams](http://blog.scoutapp.com/articles/2016/07/12/how-to-make-text-searches-in-postgresql-faster-with-trigram-similarity)
   - [Fast Search Using PostgreSQL Trigram Indexes](https://about.gitlab.com/2016/03/18/fast-search-using-postgresql-trigram-indexes/) 
   - [Awesome Autocomplete: Trigram Search in Rails and PostgreSQL](https://www.sitepoint.com/awesome-autocomplete-trigram-search-in-rails-and-postgresql/)
     - similarity, ActiveRecord::Base.connection.quote
   - [PostgreSQL扩展pg_trgm用法笔记](http://zhangwensheng.cn/blog/post/vincent/postgresql_extension_pgtrgm)
     - N-gram是计算机语言学和概率论范畴内的概念，是指给定的一段文本或语音中N个项目（item）的序列。项目（item）可以是音节、字母、单词或碱基对。通常N-grams取自文本或语料库。 
N=1时称为unigram，N=2称为bigram，N=3称为trigram，以此类推
   - [利用pg_trgm的gist和gin索引加速字符匹配查詢 ](http://blog.chinaunix.net/uid-20726500-id-4824895.html)
     - pg_trgm的工作原理是把字符串切成N個3元組，然後對這些3元組做匹配，所以如果作為查詢條件的字符串小於3個字符它就罷工了。
 - [如何用PostgreSQL解決一個人工智能語義去重的小問題](https://yq.aliyun.com/articles/25899)
 - [從難纏的模糊查詢聊開 - PostgreSQL獨門絕招之一 GIN , GiST , SP-GiST , RUM 索引原理與技術背景](https://yq.aliyun.com/articles/68244?spm=5176.100239.blogrightarea25899.18.hDJtzC)
 - [从相似度算法谈起 - Effective similarity search in PostgreSQL](https://github.com/digoal/blog/blob/master/201612/20161222_02.md?spm=5176.100239.blogcont68244.30.QI2Su0&file=20161222_02.md)
 - [Use Subqueries to Count Distinct 50X Faster](https://www.periscopedata.com/blog/use-subqueries-to-count-distinct-50x-faster.html)
 - collection
   - [談談SQL Server的定序(Collation)](https://dotblogs.com.tw/jimmyyu/archive/2009/08/30/10320.aspx)
   - [PostgreSQL Collation Support](https://www.postgresql.org/docs/9.1/static/collation.html)
   - [日本語 Solution when PostgreSQL can not properly sort strings](http://qiita.com/anoworl/items/af9f12f915b8969ea40d)
   - [HerokuのPostgresqlで日本語ソートにハマった](http://count0.org/2012/11/21/heroku-postgresql-japanese-sort.html)
 
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
 - WebSockets From Scratch
  - https://blog.pusher.com/websockets-from-scratch/
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
 - [vertical-align sample](https://jsfiddle.net/ilake/mzL7arpq/), [vertical-align-sampe-2](https://jsfiddle.net/ilake/7manafyL/)
 - [viewpoint height - Make div 100% height of browser window](http://stackoverflow.com/questions/1575141/make-div-100-height-of-browser-window)
 - [Move js event to first](http://stackoverflow.com/questions/13979961/how-do-you-force-your-javascript-event-to-run-first-regardless-of-the-order-in)
 - [glob a directory in Ruby but exclude certain directories?](http://stackoverflow.com/a/27707682/609365)
 - [xml nokogiri example](https://gist.github.com/ilake/995ccfacf452ce10984d947c1dcab4ec)
 - [xml find with namespace](http://stackoverflow.com/a/5239991/609365)
 - [What does “xmlns” in XML mean?](http://stackoverflow.com/questions/1181888/what-does-xmlns-in-xml-mean)
 - [Momentum Scrolling on iOS Overflow Elements](https://css-tricks.com/snippets/css/momentum-scrolling-on-ios-overflow-elements/)
 - [mysqldump special character issue](http://stackoverflow.com/questions/3583691/mysqldump-and-restore-with-special-characters-%C3%B8%C3%A6%C3%A5%C3%98%C3%86%C3%85)
 - [Bootstrap modal appearing under background in mobile](http://stackoverflow.com/questions/10636667/bootstrap-modal-appearing-under-background#comment54673813_11788713)
 - ios scroll disapper issue
   - [iOS 5 Native Scrolling](https://web.archive.org/web/20131005175118/http://cantina.co/2012/03/06/ios-5-native-scrolling-grins-and-gothcas/)
   - [iPad Safari scrolling causes HTML elements to disappear and reappear with a delay](http://stackoverflow.com/a/10170170/609365)
 - [iPad Safari - Make keyboard disappear](http://stackoverflow.com/questions/5937339/ipad-safari-make-keyboard-disappear)
 - heroku scale
  - [1 to 1000 - Scaling a Rails App on Heroku](https://www.joinhandshake.com/engineering/scaling/heroku/2016/01/15/1-to-1000-scaling-a-rails-app-on-heroku.html)
  - [Scaling Rails to 125,000 Requests per Minute on Heroku](https://zeemee.engineering/scaling-rails-to-125-000-requests-per-minute-on-heroku-b4128a10a769#.3wfhp3aff)
  - [git merge conflict automatic resolution]
    - git merge -s recursive -X theirs source_branch
    - git merge -Xours B

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
