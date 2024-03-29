? DCI
- DCI (Data Context Interaction) is a new way to look at object-oriented programming. Instead of focusing on individual objects, the DCI paradigm focuses on communication between objects and makes it explicit. It improves the readability of the code, which helps programmers to reason about their programs.

? SICP
- Structure and Interpretation of Computer Programs (SICP) is a textbook aiming to teach the principles of computer programming, such as abstraction in programming, metalinguistic abstraction, recursion, interpreters, and modular programming.

? Sandy Metz rules
- Classes can be no longer than one hundred lines of code.
- Methods can be no longer than five lines of code.
- Pass no more than four parameters into a method. Hash options are parameters.
- Controllers can instantiate only one object. Therefore, views can only know about one instance variable and views should only send messages to that object (@object.collaborator.value is not allowed).

? Testing
- Unit
* The first to be carried out is the unit test. As the name suggests, this method tests at the object level. Individual software components are tested for any errors. Accurate knowledge of the program is needed for this test, as each module is checked. Thus, this testing is done by the programmers and not the testers. Test codes are created to check if the software behaves as it is intended to.

- Integration
* Individual modules that are already subjected to unit testing are integrated with one another, and are tested for faults. Such a type of testing highlights interfacing errors. A 'top-down' approach of integration testing follows the architectural structure of the system. Another approach taken is the 'bottom-up' approach, which is conducted from the bottom of the control flow.

- Acceptance
* This is the last test that is conducted before the software is handed over to the client. It is carried out to ensure that the software that has been developed meets all customer requirements. There are two types of acceptance testing - one that is carried out by the members of the development team, known as internal acceptance testing (Alpha testing), and the other that is carried out by the customer, known as external acceptance testing. If the testing is carried by the intended customers, it is termed as customer acceptance testing. In case the test is performed by the end users of the software, it is known as user acceptance testing (Beta testing).

? BDD

? TDD

? Difference between BDD & TDD

? Concurrency Patterns

? NoSQL - What is the good and bad about NoSQL? What types of migrations exist ? What types of noSQL you know

? OAuth

? Cloud Orchestration
- Puppet
- Chef
- Docker

? Deploy
- Capistrano, difference between 2 and 3 version.

? Monitoring
- NewRelic

? Message Queue
- Resque, Sidekiq, different between them.

? Block, Lambda, Proc
- Procs are objects, blocks are not;
- At most one block can appear in an argument list;
- Lambdas check the number of arguments, while procs do not;
- Lambdas and procs treat the ‘return’ keyword differently;

? CSRF

? STI
- STI is when you have a parent model class that has subclasses and they store data into a single table.

react, ember, angular, backbone, Node - pros and cons

Compare Grunt, Gulp, Bower, Yeoman, Asset Pipeline, NPM

How do you generate documentation ?

Compare Delayed job, Resque, Sidekick

What is the difference between Thread and Fiber?

How to work with Graphs, Trees, Mind Map (database, ruby, frontend)

What charting libraries do you use (D3, Google chart)


What image/video processing tools do you know

What 3rd party services did you use ?

How to authorize user to see image on S3. How to restrict access?

How to implement infinite scroll

What is data segregation, sharding?

What is multi-tenancy ?

Draw a diagram for integration of two APIs?

what http request clients do you know?

What is functional reactive programming (FRP) applied to Ruby stack

----

блок, посты->комментарии.
поиск слова в посте или в комментарии.
если постгрес, если мускул, способ поиска, индекс.

Индекс для постгреса: полнотекстовые индексы
дефолт скоупы (плохо) - модель может выбираться в разных контекстах, если юзаешь всякие рейк таски, сервисы
open-close - открыт для расширения, закрыт для модификации. Когда дизайнишь архитектуру.

если js-amd arc.
распределенные паттерны?
treaty-safe, mutex, semaphore

sitekiq, resque (1 tread)

3rd party API, rate-limit: 100 queries.
redis

какая разница между второй и третий (более независимая) капистрано.

vcr
контроллер, вью, роутинг тест.
nosql - mongo (документно ориентируемая), отсутствие схемы,
типы nosql (key=>value), kasandra (column oriented), neo4j.

redis - в память пишет, в монго - на диск.
что можно мониторить в руби приложение - newrelic, airbrake

вопрос о oauth, провайдер (доверенное лицо) - шлет клиент сикрет - на провайдер с логином и паролем, провайдер выдает юзеру на этот клиент токент - акксесс токен или фреш токен. Остальные запросы через акксесс токен. Рефреш токен не экспайрится.

авторизация (проверяет на доступ) vs аутентикация (проверяет кто такой юзер)

http://en.wikipedia.org/wiki/CAP_theorem
message quequ-eventmachine, rabitmq, zeromq - продюсер пишет в quequ, консьюмеры подписываются по ключу,

publisher subscriber
разница между fiber (лямбда-тред) and tread
Fibur

тулзы для управления ассетами - спрокеты,

cloud orchestration - chef (слишком универсальные), docker
https://www.ibm.com/developerworks/community/blogs/e3ec7365-1b09-44f2-906f-19826275860f/entry/what_is_cloud_orchestration_how_can_it_help_simplify_and_accelerate_service_delivery2?lang=ru

что такое дерево - acts_as_tree
что такое граф, сильно связанные и нет,

batch, mindmap
pagination - limit, offset
Index - gist index (когда данные строятся часто, но не хорошо), gin index (когда данные редко обновляются, строятся хорошо)
data sharding (разложение данных на N сервер)

multi-tenancy
https://leanpub.com/multi-tenancy-rails

https://hackpad.com/DataXu-Senior-Software-Engineer-Ruby-7azeb2PQlw8


----


DataXu - Senior Software Engineer (Ruby)

WANTED
Ruby backend-oriented developer to join our team working on the next generation of industry-leading Digital Marketing Management platform at dataxu.com

Team
We   are team of senior developers, work in agile and remote environment,   and our aim is to deliver high-quality product in-time. We are proud of   our work and use all modern dev processes, like code reviews,  workshops,  hangouts, pair programming, CI, to deliver extensible and  scalable  modules for further use. Across whole product branches, we  keep teams  small, up to 4 people, to maximize productivity and quality  of our  solutions.

Backend Stack
Product core is set of Java/Scala modules that manage real-time (single digit millisecond responses) big-data (terabytes daily) high-load (up to 700K requests/sec recently) flow.

Current Ruby layer sits on top of PostgreSQL DB with aggregated big-data:
MRI 2.x, RoR 4.x, Sinatra etc
Some servers in some datacenters managed by dedicated DevOps team
Several API, aim to split data into up to 20 API, public and private
250+ entities, ActiveRecord and other
appropriate number of controllers, decorators, data validators, generators, libs, report builders, various gems to import and export data, custom gems
PG, Solr, Facebook libs, Google libs, memcache, redis, various auth-related gems, sunspot,  chronic, google-spreadsheet-ruby, highline, nokogiri, roo, vast, delayed_job, carrierwave, ffmpeg, vestal_versions, CodeClimate, Newrelic, rspec, capybara
other scripts with Python and Bash

You will
As part of the CORE engineering team, contribute to design and implementation as required to deliver complete, complex, new highly scalable enterprise level capabilities.
Be part of team of professionals, learn a lot from each other and improve skills together.
Develop new RESTful services consumed by all DataXu engineering groups, 3rd party companies and clients.
Make difference, design and implement best backend architecture solutions
Contribute to the R&D and build-out of future systems
Solve interesting & complex problems, such as scaling applications for large data computation and reporting
Build a very scalable high performance API layer
Try out edge technologies in real-time big-data hi-load fields
Add new functionality to existing systems, while constantly improving usability and quality
Avoid accidental complexities at scale
Implement unit, component and integration tests to cover new functionality
Report to Product Manager and Sr Director for Engineering

About Product
We help leading advertisers manage their online advertising campaigns across all (mobile, web, TV) media channels, device platforms and advertising exchanges. We help small advertising agencies forecast their audience, providing various geo- and behavior-based reports for different industries.

Product Features
Real-time ad bidding and content delivery requires single-digit millisecond responses, guided by machine learning. We use real rocket science to manage data collection from various channels, generate AI-based forecasting and make decisions on what user will like and think about,  when he opens publisher's website.

Minimum Developer Requirements
Very strong engineering principles for building horizontally scalable servers/services with strong reliability and high performance.
Extensive knowledge of Ruby stack
Proven success with SOA, specifically developing REST services (JSON or XML over HTTP) using any technology (Ruby, Java, C, etc.)
Experience building and supporting enterprise high-availability 24/7 systems
A passion for delivering high quality solutions. Experience with continuous integration and test automation.
Extensive experience with relational data modeling, databases and SQL
Must love to learn new technologies
Strong verbal, written and team-oriented communication skills