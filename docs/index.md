

# (WORK IN PROGRESS) Zero Backend (Øb)

I was bored building and managing custom backends, so i built this.

Øb will redefine the way you think about backend and backoffice code.



## What can you build with Øb ?

First, you start by defining your data, then you add backend/backoffice features to your site.

Since you shape your own data, there are few limits to what you can build.

With this features, you could for example build:

* ecommerce web site
* blog / magazine
* professional folio
* corporate website
* real estate agency site
* agency site/folio
* restaurant website with online booking
* clinic website with online appointment booking
* events website with participation booking
* coupon website
* marketplace
* dashboard for your client (we call it middleoffice)

More importantly, you can combine it all together. Let's say you want to build an eshop with a blog. Well, no issues there, it works perfectly together. 


## Who is it for ?

**full stack developpers**

* who care about delivering faster results to their clients
* will discover new way of managing backend stack


**frontend developpers**

* who don't want to write backend code
* will be able to build somewhat complex web sites with Ø backend code


## Static by default

With classic set of full stack and backend frameworks, we usualy make every page dynamic by default, even if it doesn't have to be.

Because of everything is dynamic, we have to worry about things like:

* scaling / caching / optimisations
* security
* server infrastructure
* monitoring
* backups / disaster recovery
* ...

ZeroBackend uses static generated approach by default, and implements dynamic features as services.

Services = Hosted, fully managed services with REST APIs and production ready client libraries.

Each service has it's own backoffice to manage data.


To design ZeroBackend, we considered many use cases. Please check our case studies:

* [Case Study: Small to Medium size Eshop](case-study/eshop)
* [Case Study: Blog](case-study/blog)
* more to come...




## Not your your grandma's CMS

Authors of ZeroBackend hate pretty much any open source CMS with passion for many technical reasons.

A lot of efforts were put into ZeroBackend to avoid errors made by packages like Wordpress, Prestashop or Magento.

We also tried to avoid **the boring steps** found in modern frameworks, so you can enjoy the development process.

Here are few principles we care about:

* Øb user must **never** touch the backend and backoffice code
* Øb user can customize frontoffice from A to Z
* Øb doesn't assume the structure of your data, you define it yourself
* Øb generates API in real time for each data entity you create, so advanced users can easily use their data from anywhere
* Øb frees you from managing a database, servers, backups, ...
* Øb will host your static site. But you can also host it yourself, if you wish.
* Øb plays well with other backed as service. Want to use Disqus for your comments or Firebase for realtime communications ? No problem, it just works
* Øb takes care of the Backend code, APIs and Backoffice UIs.
* Øb provides you a powerful static site generator. However you can use your own if you wish, simply plug to our APIs and start building.
* You do the frontend (don't worry, we have project templates to get you started)


