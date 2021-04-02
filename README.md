http://localhost:4200/auth/login


Auth Login
1.- public/authentication.actions.ts  			(Actions)
2.- public/authentication/login/login.component.ts 	(Disparador de dispatch)
3.- public/authentication/authentication.effects     	(Efecto)

4.- El efecto guarda token en cookie y envia datos simples al reducer.


Users Me
1.- private/users/users.actions  			(Actions)
2.- app/application.service 				(Disparador de dispatch antes que se inicie la app, basado en token)
3.- private/users/users.effects				(Efecto de users/me)
4.- private/users/users.reducers			(Asignacion de data, user, selectedClient, availableClients)

En el proceso anterior, cada F5 asegura que tengamos en el store, el selectedClient, availableClient y userDetails


http://localhost:4200/choose-project

Choose Project
1.- private\projects\projects.actions.ts		(Actions)
2.- private\private-header\private-header.component.ts	(Disparador de dispatch, cambiante)
3.- private\projects\projects.effects.ts		(Efectos)

4.- private\projects\choose-project\choose-project.component.ts		(Table final)