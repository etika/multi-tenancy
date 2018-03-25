# Multi-Tenancy

This small repository was created to reproduce an example of usage of apartment gem.
It has two models (User and Project) to show how multi-tenancy actually works.

### Testing
* start installing all the dependencies
``` bundle ```

* raise the server
``` rails server ```

* let's use lvh.me so it will allow to test subdomains locally. *lvh simulates localhost
lvh.me:3000/users.

* in order to see the differences create two users.

* then use the subdomain. Eg: **subdomain**.lvh:3000/projects.

* create a project and then switch to another user domain
there will be only the respective projects, because apartment gem automatically separate tables from each tenant.

it's great \o/
