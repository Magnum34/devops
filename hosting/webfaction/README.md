# Webfactional

## Required

* ansible

https://docs.ansible.com/ansible/latest/installation_guide/intro_installation.html

## Change variables
Next, copy the hosts.example file and change to your Webfaction account name.
```
cp hosts.example hosts
nano hosts
```
Similarly, copy the vars/external_vars.yml file and change all values to your liking. 
```
cd vars
cp external_vars.yml.example external_vars.yml
nano external_vars.yml
```
## Type Stage

* Stage Wordpress - create-stage-wordpress.yml
* Stage Laravel - create-stage-laravel.yml
* Stage SilverStripe 4 - create-stage-silverstripe.yml

TODO:

* Stage NodeJS 
* Stage Django

## Usage
Can be made server or remote. :)

Now execute the playbook:
```
ansible-playbook -i hosts create-stage-wordpress.yml

```

If you have correctly setup your Website in the webfaction panel, you should be able to see your project now if you visit http://username.webfactional.com.