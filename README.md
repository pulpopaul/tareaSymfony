tareita
=======

A Symfony project created on July 28, 2016, 2:13 am.

pulpo@pulpo-HP-Compaq-nx6320-RN828LA-ABM:~/symfonyProjects/tareita$ composer require triton/crud-generator
Using version ^1.0 for triton/crud-generator
./composer.json has been updated
Loading composer repositories with package information
Updating dependencies (including require-dev)
  - Installing lexik/form-filter-bundle (v5.0.1)
    Loading from cache

  - Installing pagerfanta/pagerfanta (v1.0.3)
    Loading from cache

  - Installing triton/crud-generator (1.0.3)
    Loading from cache

pagerfanta/pagerfanta suggests installing mandango/mandango (To use the MandangoAdapter.)
pagerfanta/pagerfanta suggests installing doctrine/mongodb-odm (To use the DoctrineODMMongoDBAdapter.)
pagerfanta/pagerfanta suggests installing doctrine/phpcr-odm (To use the DoctrineODMPhpcrAdapter. >= 1.1.0)
pagerfanta/pagerfanta suggests installing propel/propel1 (To use the PropelAdapter)
pagerfanta/pagerfanta suggests installing solarium/solarium (To use the SolariumAdapter.)
Writing lock file
Generating autoload files
> Incenteev\ParameterHandler\ScriptHandler::buildParameters
Updating the "app/config/parameters.yml" file
> Sensio\Bundle\DistributionBundle\Composer\ScriptHandler::buildBootstrap
> Sensio\Bundle\DistributionBundle\Composer\ScriptHandler::clearCache

 // Clearing the cache for the dev environment with debug true                                                          


 [OK] Cache for the "dev" environment (debug=true) was successfully cleared.                                            


> Sensio\Bundle\DistributionBundle\Composer\ScriptHandler::installAssets

 Trying to install assets as relative symbolic links.

 --- ----------------- ------------------ 
      Bundle            Method / Error    
 --- ----------------- ------------------ 
  ✔   FrameworkBundle   relative symlink  
 --- ----------------- ------------------ 


 [OK] All assets were successfully installed.                                                                           


> Sensio\Bundle\DistributionBundle\Composer\ScriptHandler::installRequirementsFile
> Sensio\Bundle\DistributionBundle\Composer\ScriptHandler::prepareDeploymentTarget
pulpo@pulpo-HP-Compaq-nx6320-RN828LA-ABM:~/symfonyProjects/tareita$ php app/console generate:bundle --name=PabloTareaBundle

                                                          
  [Symfony\Component\Console\Exception\RuntimeException]  
  The "--name" option does not exist.                     
                                                          

generate:bundle [--namespace NAMESPACE] [--dir DIR] [--bundle-name BUNDLE-NAME] [--format FORMAT] [--shared] [-h|--help] [-q|--quiet] [-v|vv|vvv|--verbose] [-V|--version] [--ansi] [--no-ansi] [-n|--no-interaction] [-s|--shell] [--process-isolation] [-e|--env ENV] [--no-debug] [--] <command>

pulpo@pulpo-HP-Compaq-nx6320-RN828LA-ABM:~/symfonyProjects/tareita$ php app/console generate:bundle --bundle-name=PabloTareaBundle

                                            
  Welcome to the Symfony bundle generator!  
                                            

Are you planning on sharing this bundle across multiple applications? [no]:  

Your application code must be written in bundles. This command helps
you generate them easily.

Give your bundle a descriptive name, like BlogBundle.
Bundle name: PabloTareaBundle

Bundles are usually generated into the src/ directory. Unless you're
doing something custom, hit enter to keep this default!

Target Directory [src/]: 

What format do you want to use for your generated configuration?

Configuration format (annotation, yml, xml, php) [annotation]: 

                     
  Bundle generation  
                     

> Generating a sample bundle skeleton into app/../src/PabloTareaBundle OK!
> Checking that the bundle is autoloaded: OK
> Enabling the bundle inside app/AppKernel.php: OK
> Importing the bundle's routes from the app/config/routing.yml file: OK
> Importing the bundle's services.yml from the app/config/config.yml file: OK

                                         
  Everything is OK! Now get to work :).  
                                         

pulpo@pulpo-HP-Compaq-nx6320-RN828LA-ABM:~/symfonyProjects/tareita$ $ php bin/console doctrine:database:create
$: command not found
pulpo@pulpo-HP-Compaq-nx6320-RN828LA-ABM:~/symfonyProjects/tareita$ php app/console doctrine:database:create

                                                                               
  [Doctrine\DBAL\Exception\ConnectionException]                                
  An exception occured in driver: SQLSTATE[28000] [1045] Access denied for us  
  er 'root'@'localhost' (using password: NO)                                   
                                                                               

                                                                               
  [Doctrine\DBAL\Driver\PDOException]                                          
  SQLSTATE[28000] [1045] Access denied for user 'root'@'localhost' (using pas  
  sword: NO)                                                                   
                                                                               

                                                                               
  [PDOException]                                                               
  SQLSTATE[28000] [1045] Access denied for user 'root'@'localhost' (using pas  
  sword: NO)                                                                   
                                                                               

doctrine:database:create [--connection [CONNECTION]] [--if-not-exists] [-h|--help] [-q|--quiet] [-v|vv|vvv|--verbose] [-V|--version] [--ansi] [--no-ansi] [-n|--no-interaction] [-s|--shell] [--process-isolation] [-e|--env ENV] [--no-debug] [--] <command>

pulpo@pulpo-HP-Compaq-nx6320-RN828LA-ABM:~/symfonyProjects/tareita$ php app/console doctrine:database:create

                                                                                                                         
  [Doctrine\DBAL\Exception\ConnectionException]                                                                          
  An exception occured in driver: SQLSTATE[28000] [1045] Access denied for user 'root'@'localhost' (using password: NO)  
                                                                                                                         

                                                                                         
  [Doctrine\DBAL\Driver\PDOException]                                                    
  SQLSTATE[28000] [1045] Access denied for user 'root'@'localhost' (using password: NO)  
                                                                                         

                                                                                         
  [PDOException]                                                                         
  SQLSTATE[28000] [1045] Access denied for user 'root'@'localhost' (using password: NO)  
                                                                                         

doctrine:database:create [--connection [CONNECTION]] [--if-not-exists] [-h|--help] [-q|--quiet] [-v|vv|vvv|--verbose] [-V|--version] [--ansi] [--no-ansi] [-n|--no-interaction] [-s|--shell] [--process-isolation] [-e|--env ENV] [--no-debug] [--] <command>

pulpo@pulpo-HP-Compaq-nx6320-RN828LA-ABM:~/symfonyProjects/tareita$ php app/console doctrine:database:create
Created database `spabloTarea` for connection named default
pulpo@pulpo-HP-Compaq-nx6320-RN828LA-ABM:~/symfonyProjects/tareita$ php app/console doctrine:generate:entity

                                             
  Welcome to the Doctrine2 entity generator  
                                             


This command helps you generate Doctrine2 entities.

First, you need to give the entity name you want to generate.
You must use the shortcut notation like AcmeBlogBundle:Post.

The Entity shortcut name: PabloTareaBundle:Producto

Determine the format to use for the mapping information.

Configuration format (yml, xml, php, or annotation) [annotation]: 

Instead of starting with a blank entity, you can add some fields now.
Note that the primary key will be added automatically (named id).

Available types: array, simple_array, json_array, object, 
boolean, integer, smallint, bigint, string, text, datetime, datetimetz, 
date, time, decimal, float, binary, blob, guid.

New field name (press <return> to stop adding fields): name
Field type [string]: 
Field length [255]: 
Is nullable [false]: 
Unique [false]: 

New field name (press <return> to stop adding fields): 

                     
  Entity generation  
                     

> Generating entity class src/PabloTareaBundle/Entity/Producto.php: OK!
> Generating repository class src/PabloTareaBundle/Repository/ProductoRepository.php: OK!

                                         
  Everything is OK! Now get to work :).  
                                         

pulpo@pulpo-HP-Compaq-nx6320-RN828LA-ABM:~/symfonyProjects/tareita$ php app/console generate:doctrine:crud --entity=PabloTareaBundle:Producto

                                           
  Welcome to the Doctrine2 CRUD generator  
                                           


This command helps you generate CRUD controllers and templates.

First, give the name of the existing entity for which you want to generate a CRUD
(use the shortcut notation like AcmeBlogBundle:Post)

The Entity shortcut name [PabloTareaBundle:Producto]: 

By default, the generator creates two actions: list and show.
You can also ask it to generate "write" actions: new, update, and delete.

Do you want to generate the "write" actions [no]? yes     

Determine the format to use for the generated CRUD.

Configuration format (yml, xml, php, or annotation) [annotation]: 

Determine the routes prefix (all the routes will be "mounted" under this
prefix: /prefix/, /prefix/new, ...).

Routes prefix [/producto]: 

                             
  Summary before generation  
                             

You are going to generate a CRUD controller for "PabloTareaBundle:Producto"
using the "annotation" format.

Do you confirm generation [yes]? 

                   
  CRUD generation  
                   

Generating the CRUD code: OK
Generating the Form code: OK
Updating the routing: OK

                                         
  Everything is OK! Now get to work :).  
                                         

pulpo@pulpo-HP-Compaq-nx6320-RN828LA-ABM:~/symfonyProjects/tareita$ 

