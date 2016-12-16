# Zenphoto-Vagrant

Buenas.

Para poder darle uso a este proyecto deben constar de lo siguiente:
  Vagrant 1.8.6
       +sus paquetes de ruby y virtualbox
  Ubuntu como sistema anfitrión (16 en mi caso)
  
  
  
Descargar la box
        Posibilidades:
          https://drive.google.com/file/d/0B4FIs0XjkjNgeUJUTDcwSTNza1E/view
          https://mega.nz/#!yIUjBIQB!1nFihgCC1e7FW2Vb_XJQVXM_kNyyxAjkR0pI93e0wZM
          
          wget
              #esta box ha partido de una ubuntu/trusty64 mas los añadidos de un stack LAMP
          
    Añadir dicha box a vuestra lista de cajas.
        vagrant box add /rutadedescarga/package.box --name Nombre
           #rutadescarga    deberia ser la ruta  actual o doonde este descargada la bos que he subido
           #Nombre se sustituye por el nombre a vuestro gusto, solo tener en cuenta que es el que hay que usar en vuestro Vagrantfile
           
   Crear un Vagrantfile
      mkdir carpetabox
      cd carpetabox
      vagrant init
      nano Vagrantfile
      
      
          En este debeis añadir como base el nombre que le dsiteis a la box y añadir un adaptador de red, aconsejable que sea publico, tal como el ejemplo de Vagrantfile que he subido.
          
     Una vez realizado el vagrant up solo debereis abrir vuestro navegador y usar la ip asignada en el adaptador de esta manera
              http://192.168.0.5/html/zenphoto/
              
       Usuario administrador    Admin     pass  X
       
     Tiene el tema cambiado y algunas fotos interesantes que han salido de goodfon.ru por parte de unos usuarios muy inspirados.
   
