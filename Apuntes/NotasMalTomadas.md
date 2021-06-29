#  En esta sección podrá encontrar diferentes notas que no tiene un orden y formato. 
La intención de apartado es encotrar varios ejemplos practicos que puedan ser de mucha utilidad.

* Interpolación en JavaScrit

```typescript
console.log(`I'm ${age} years old!`)

this.project.responsiblesNotification.forEach(responsible=>{
       let messaj=`¡Hola ${responsible.responsibleUserId} ! Te queremos comentar que 
                    Valentina Maza marcó a la oportunidad `; 
       
});

```

* Crear un objeto de un interface para add arreglo objeto

```typescript
getResponsibleNotification(){ 
   this.project.responsiblesNotification=[] ;
   this.responsibleNotifications.forEach(user=>{
      let dato: ResponsibleNotification = {}; 
      dato.responsibleUserId=user.id         
      this.project.responsiblesNotification.push(dato); 
   });   
}

```

* Add un elemento en un array

```typescript
setNotificacionOpportunityProject(): void{

    let userNotifications: UserNotification[] = [];
 
    this.project.responsiblesNotification.forEach(responsible=>{      
        let userNotification: UserNotification = {};      
        userNotification.instanceId=this.opportunity.instanceId;;
        userNotification.isActive=true;
        userNotification.notification=notification;
        userNotification.applicationUser=applicationUser;
        userNotifications.push(userNotification); 
  });
```
* Subscribe return null

```typescript
  this.notificationService.newNotificationOpportunityProject(userNotifications,this.opportunity.instanceId).subscribe(
       ()=>{},erro=>console.log(erro));
```

* Ejemplo de como validar con una expresión regular una url para que anteceda http, ftp, https
```typescript
  validLink(): boolean {
    if(this.newLink.name == null || this.newLink.name == "") { return false; }
    let regex = new RegExp(/^(ftp|http|https):\/\/[^ "]+$/)
    if(!regex.test(this.newLink.urlLink)){ return false; }
    if(this.newLink.urlLink == null || this.newLink.urlLink == "") { return false; }
    return true;
  }
```

