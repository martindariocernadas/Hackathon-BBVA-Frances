# bbva-frances-hackathon


Hackathon-BBVA-Frances
----------------------
Evento en EventBrite        : https://www.eventbrite.com/e/hackathon-bbva-frances-buenos-aires-octubre-2017-tickets-36322832570
Repo en Github              : https://github.com/martindariocernadas/Hackathon-BBVA-Frances
Amazon S3 bucket            : ("hackaton-bbva-frances")
Amazon CodeBuild (Jenkins)  : ("buildspec.yml")


Para administradores : COMO CONECTAR al servicio PaaS-Jenkins de AMAZON contra el repositorio Github 
----------------------------------------------------------------------------------------------------

AWS Console :               : https://console.aws.amazon.com/console/home
                                Login a AWS Console (con su usuario validado y con permisos a AmazonS3 + CodeBuild)
 
Amazon S3 bucket            : https://aws.amazon.com/s3/ 
                                Definir un Bucket de persistencia ( "hackaton-bbva-frances" )
                                URL: https://s3.console.aws.amazon.com/s3/buckets/hackathon-bbva-frances/?region=us-west-2&tab=overview                              
Amazon CodeBuild (Jenkins)  : https://aws.amazon.com/codebuild/ 
                                Definir un Proyecto de construccion CodeBuild ( "Hackathon-BBVA-Frances" )
                                Project name: "Hackathon-BBVA-Frances"
                                Source provider: "GitHub"
                                Repository: (ej. https://github.com/martindariocernadas/Hackathon-BBVA-Frances)
                                Artifact type: "Amazon S3"
                                Artifact name: "Hackathon-BBVA-Frances"
                                Artifact packaging: "Zip"
                                
                                URL: https://us-west-2.console.aws.amazon.com/codebuild/home?region=us-west-2#/projects/Hackathon-BBVA-Frances/view
                                
                                Darle BUILD ...
                                Esperar la finalizacion y ver los resultados del LOG.
                                

