# README

![](https://cp5.sgp1.cdn.digitaloceanspaces.com/zoro/laravue-cdn/laravue-logo-line.png)

 [![vue](https://img.shields.io/badge/laravel-7.3-brightgreen.svg)](https://laravel.com) [![vue](https://img.shields.io/badge/vue-2.6.10-brightgreen.svg)](https://github.com/vuejs/vue) [![element-ui](https://img.shields.io/badge/element--ui-2.13.0-brightgreen.svg)](https://github.com/ElemeFE/element) [![license](https://img.shields.io/badge/license-MIT-brightgreen.svg)](https://github.com/tuandm/laravue/blob/master/LICENSE)

## Laravue

[Laravue](https://laravue.dev) \(pronounced /ˈlarəvjuː/\) is a beautiful dashboard combination of [Laravel](https://laravel.com/), [Vue.js](https://github.com/vuejs/vue) and the UI Toolkit [Element](https://github.com/ElemeFE/element). The work is inspired by [vue-element-admin](http://panjiachen.github.io/vue-element-admin) with our love on top of that. With the powerful Laravel framework as the backend, Vue.js as the high performance on the frontend, Laravue appears to be a full-stack solution for an enterprise application level.

Documentation: [https://doc.laravue.dev](https://doc.laravue.dev)

### Screenshot

![](https://cdn.laravue.dev/screenshot.png)

### Getting started

#### Prerequisites

* Laravue is positioned as an enterprise management solution, and it is highly recommended to use it to start from scratch.
* For existing Laravel project, you should check [Laravue Core](https://github.com/tuandm/laravue-core) for integration.
* Your machine needs to be ready for the latest [Laravel](https://laravel.com/docs/6.x#installation) and [Node.js](https://nodejs.org).

#### Installing

**Manual**

```bash
# Clone the project and run composer
composer create-project tuandm/laravue
cd laravue

# Migration and DB seeder (after changing your DB settings in .env)
php artisan migrate --seed

# Install dependency with NPM
npm install

# develop
npm run dev # or npm run watch

# Build on production
npm run production
```

**Docker**

```bash
docker-compose up -d
```

Build static files within Laravel container with npm

```bash
# Get laravel docker container ID from containers list
docker ps

docker exec -it <container ID> npm run dev # or npm run watch
# Where <container ID> is the "laravel" container name, ex: src_laravel_1
```

Open [http://localhost:8000](http://localhost:8000) \(laravel container port declared in `docker-compose.yml`\) to access Laravue

### Running the tests

* Tests system is under development

### Deployment and/or CI/CD

This project uses [Envoy](https://laravel.com/docs/5.8/envoy) for deployment, and [GitLab CI/CD](https://about.gitlab.com/product/continuous-integration/). Please check `Envoy.blade.php` and `.gitlab-ci.yml` for more detail.

### Built with

* [Laravel](https://laravel.com/) - The PHP Framework For Web Artisans
* [Laravel Sanctum](https://github.com/laravel/sanctum/) - Laravel Sanctum provides a featherweight authentication system for SPAs and simple APIs.
* [spatie/laravel-permission](https://github.com/spatie/laravel-permission) - Associate users with permissions and roles.
* [VueJS](https://vuejs.org/) - The Progressive JavaScript Framework
* [Element](https://element.eleme.io/) - A  Vue 2.0 based component library for developers, designers and product managers
* [Vue Admin Template](https://github.com/PanJiaChen/vue-admin-template) - A minimal vue admin template with Element UI

### Contributing

Please read [CONTRIBUTING.md](contributing.md) for details on our code of conduct, and the process for submitting pull requests to us.

### Versioning

We use [SemVer](http://semver.org/) for versioning. For the versions available, please look at the [release tags](https://github.com/tuandm/laravue/tags) on this repository.

### Authors

* **Tuan Duong** - _Initial work_ - [tuandm](https://github.com/tuandm).
* **Tony Tin Nguyen** - _Frontend and Designer_ - [nguyenquangtin](https://github.com/nguyenquangtin).

See also the list of [contributors](https://github.com/tuandm/laravue/contributors) who participated in this project.

### License

This project is licensed under the MIT License - see the [LICENSE.md](https://github.com/FHARIS2019/laravue/tree/f5c227bac0199479b5e1abfb70f307b21ff65032/LICENSE/README.md) file for details.

### Related projects

* [Laravue-core](https://github.com/tuandm/laravue-core) - Laravel package which provides core functionalities of Laravue.

### Acknowledgements

* [vue-element-admin](https://panjiachen.github.io/vue-element-admin/#/) A magical vue admin which insprited Laravue project.
* [tui.editor](https://github.com/nhnent/tui.editor) - Markdown WYSIWYG Editor.
* [Echarts](http://echarts.apache.org/) - A powerful, interactive charting and visualization library for browser.

### Donate

If you find this project useful, you can [buy me a coffee](https://www.buymeacoffee.com/tuandm)

