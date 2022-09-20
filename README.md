https://learn.microsoft.com/es-mx/training/modules/azure-ad-privileged-identity-management/

## Tarea 1: Azure AD PIM para roles

En esta tarea, vamos a configurar las opciones de activación de PIM, agregar Administrador de facturación como un rol de PIM, activar el rol y probar la activación.

### CONFIGURACION DE PIM

Nota: Esta tarea requiere una cuenta AZ500User1 sin roles asignados.

En esta tarea, se revisarán los valores básicos de PIM y se configurarán.

1. En Portal, busque y seleccione Azure AD Privileged Identity Management.

2. En Administrar, seleccione Roles de Azure AD.

3. En Administrar, seleccione Configuración.

4. Seleccione el rol Administrador de facturación.

![image](https://user-images.githubusercontent.com/110675810/189480180-fc027c5e-8420-4dea-93c0-df8d5fb0f6c6.png)

5. Haga clic en Editar.

6. Observe las pestañas Activación, Asignación y Notificación.

7. De manera predeterminada, se necesita MFA para la activación. Para esta demostración, cambie el requisito a Ninguno.

8. Seleccione la casilla Se requiere aprobación para activar.

![image](https://user-images.githubusercontent.com/110675810/189480302-963ee2be-abaf-4789-b52f-dcbb53f2fca1.png)

9. Analice las otras opciones posibles, incluidas Duración máxima de la activación y Se requiere aprobación para activar.

10. Cambie a la pestaña Asignación y consulte la configuración.

11. Observe la posibilidad de hacer que expiren las asignaciones elegibles y activas.

12. Cambie a la pestaña Notificaciones y analice la configuración.

![image](https://user-images.githubusercontent.com/110675810/189480363-711e62ee-8b43-45ae-a528-c5d6624ecfcf.png)

13. Tenga en cuenta que puede enviar notificaciones al asignar miembros y activarlo.

![image](https://user-images.githubusercontent.com/110675810/189480415-53bd64fb-7f5c-499d-abca-60a03d80ad68.png)

14. Haga clic en Update(Actualizar).

![image](https://user-images.githubusercontent.com/110675810/189480437-c6487abd-813c-4020-8d4f-57c32202f6d5.png)


### CONFIGURACION DE PIM PARA LOS ROLES 

En esta tarea, se agregará el rol Administrador de facturación a PIM.

1. En Portal, busque y seleccione Azure AD Privileged Identity Management.

2. En Administrar, seleccione Roles de Azure AD.

3. EnAdministrar, seleccione Roles.

4. Revise la lista de roles.

5. Seleccione el rol Administrador de facturación.

![image](https://user-images.githubusercontent.com/110675810/189480594-3cc90b98-c2d2-4f74-831b-617e526c06d0.png)

6. Revise Roles elegibles y Roles activos.

7. Haga clic en Agregar miembro.

8. Haga clic en Seleccionar miembro y en Seleccionar para el usuario AZ500User1. Ahora es un Administrador de facturación.

![image](https://user-images.githubusercontent.com/110675810/189480723-1222a32b-74a1-4278-ab41-11c132cc73e2.png)

9. Seleccione Establezca la configuración de pertenencia. Observe que la configuración puede ser permanente o tener una limitación temporal.

- Tipo de asignación: Apto

- Elegibilidad permanente: seleccione la casilla.

10. Seleccione Guardar para los cambios y elija Agregar la asignación.

![image](https://user-images.githubusercontent.com/110675810/189480762-25978556-25b4-4119-95eb-6e09b43d9ade.png)

11. Compruebe que el Administrador de facturación aparezca como un rol elegible.

![image](https://user-images.githubusercontent.com/110675810/189480802-5254efb2-e748-493d-b1be-012be2f9e515.png)

![image](https://user-images.githubusercontent.com/110675810/189481087-6dada50f-b35b-4526-a0ba-589422cb4164.png)


### ACIVACION DE UN ROL

En esta tarea, vamos a activar el rol Administrador de facturación.

1. En el Portal, busque Azure Active Directory y selecciónelo.

2. En Administrar, haga clic en Usuarios.

3. Seleccione AZ500User1.

![image](https://user-images.githubusercontent.com/110675810/191140179-475d3dda-be1d-4926-ac0e-fa20cc064eb3.png)

4. En Administrar, haga clic en Roles asignados.

5. Compruebe que el usuario no esté asignado a ningún rol.

![image](https://user-images.githubusercontent.com/110675810/191140484-b6295e74-f516-4907-bab4-ba3b192fee6e.png)

6. Inicie sesión en Portal como AZ500User1.

7. Busque y seleccione Azure AD Privileged Identity Management.

8. En Tareas, seleccione Mis roles.

![image](https://user-images.githubusercontent.com/110675810/191140568-5c81ed45-51cf-4f55-9d23-cc0ea3c441fa.png)

9. En Activar, seleccione Roles de Azure AD.

10. Seleccione los Roles activos y compruebe que no aparezcan roles.

![image](https://user-images.githubusercontent.com/110675810/191140668-ac54f7af-5f92-4a4b-a7d7-ed9437b3568e.png)

11. En la pestaña Roles elegibles, observe el rol Administrador de facturación.

12. En la columna Acción, seleccione Activar.

![image](https://user-images.githubusercontent.com/110675810/191140958-b84c6325-4a8e-4914-9f2e-f76b5aa2aa55.png)

13. La opción de Detalles de asignación se muestra en el portal. Entre estos se incluyen las horas de inicio y finalización y la posibilidad de agregar un motivo.

14. Agregue un motivo y, a continuación, haga clic en Activar.

![image](https://user-images.githubusercontent.com/110675810/191141075-293aa09a-62f7-4bca-a384-5502e7bbdc6a.png)

15.El Estado de activación debe mostrar que se han completado todas las fases de activación.

16. Use el vínculo para Cerrar sesión.

![image](https://user-images.githubusercontent.com/110675810/191141235-ef693d8f-b3b7-44c8-a374-04ddfc3388cb.png)

17. Debe cerrar la sesión y volver a iniciarla para empezar a usar el rol recién activado.


### PRUEBA DE ACCESO AL ROL

En esta tarea, pruebe el rol Administrador de facturación.

1. Inicie sesión en el portal como AZ500User1.

![image](https://user-images.githubusercontent.com/110675810/189481860-6bdf2ca8-f53c-435a-9f95-b6f8bd8a73ff.png)

2. Busque y seleccione Azure AD Privileged Identity Management.

3. En Activar, seleccione Roles de Azure AD.

![image](https://user-images.githubusercontent.com/110675810/189482209-b456c3c0-46d8-42ee-8b97-9c689a84a60e.png)

4. Seleccione la pestaña Roles activos y compruebe que el rol Administrador de facturación se haya activado.

![image](https://user-images.githubusercontent.com/110675810/189482252-4e1ae2c7-1103-4855-8176-cf478823734f.png)

5. El rol debería aparecer ahora como Activado.

6. Observe que existe la opción de Desactivar el rol.

![image](https://user-images.githubusercontent.com/110675810/191142310-ac594442-fecc-4000-b511-b698c14be650.png)

Nota: Se puede cancelar solicitud

## Tarea:2 Azure AD PIM para recursos

En esta tarea, vamos a configurar PIM para los recursos de Azure, activaremos el rol Colaborador de la máquina virtual y probaremos el acceso al rol.

### CONFIGURACION DE PIM PARA LOS RECURSOS DE AZURE 

Pre-requisito tener permisos de administrador global 
https://learn.microsoft.com/en-us/azure/role-based-access-control/elevate-access-global-admin?toc=%252fazure%252factive-directory%252fprivileged-identity-management%252ftoc.json

En esta tarea, vamos a agregar la suscripción a PIM y, después, agregaremos el rol Colaborador de la máquina virtual como rol activo.

1. En Portal, busque y seleccione Azure AD Privileged Identity Management.

2. En Administrar, seleccione Recursos de Azure.

![image](https://user-images.githubusercontent.com/110675810/191289644-45d6ddf8-0c25-4a9f-8f64-8714615fd547.png)

3. Haga clic en Detectar recursos.

4. Observe que el Estado del recurso es No administrado.

![image](https://user-images.githubusercontent.com/110675810/191289962-2f2793bd-1e32-458b-ad09-8465950f7477.png)

5. Seleccione la suscripción que quiere administrar.

![image](https://user-images.githubusercontent.com/110675810/191290254-e7cba96f-c17c-4da1-9efd-cd14029698a6.png)

6. Haga clic en Administrar recurso.
6. Haga clic en Administrar Configuraciones.

![image](https://user-images.githubusercontent.com/110675810/191296270-4b333052-aaf4-4150-b0ea-04075ae5bba7.png)

7. Haga clic en Sí para confirmar que PIM administrará todos los objetos secundarios del recurso seleccionado.

![image](https://user-images.githubusercontent.com/110675810/191296535-9d3f8f2a-529a-4dab-abf1-fd5d33abd173.png)

8. Vuelva a la hoja Recursos de Azure.

9. Seleccione su suscripción.

![image](https://user-images.githubusercontent.com/110675810/191297041-88c2d8dc-9c94-4729-9c07-791db0e0e97d.png)

10. En Administrar, haga clic en Roles.

![image](https://user-images.githubusercontent.com/110675810/191296870-25af5ee4-e1dc-4c75-bcfc-7225d86a8458.png)

11. Busque y seleccione el rol Colaborador de la máquina virtual.

![image](https://user-images.githubusercontent.com/110675810/191297385-29985595-8169-48ed-9122-0c73c4edfb53.png)

12. Haga clic en Agregar asignaciones y, a continuación, en Seleccionar miembros y agregue AZ500User1 al grupo.

![image](https://user-images.githubusercontent.com/110675810/191298553-a90fdac6-5401-4653-b456-c53ac0f61396.png)

13. En la página Configuración de pertenencia, establezca Tipo de asignación en Activo.

![image](https://user-images.githubusercontent.com/110675810/191298630-85486d92-fd8a-4444-83b6-0747180a37a1.png)

14. Seleccione Agregar el rol y Guardar los cambios.

![image](https://user-images.githubusercontent.com/110675810/191298805-8494a843-bec3-4edb-8fc0-c70a2b460a88.png)

15. Cierre la sesión en el portal.


### ACTIVACION DEL ROL

En esta tarea, vamos a iniciar sesión como usuario y activaremos el rol.

![image](https://user-images.githubusercontent.com/110675810/191299532-5493c1c0-f455-438c-a590-fd201314bb28.png)

1. Inicie sesión en el Portal y en AZ500User1.

2. Busque y seleccione Azure AD Privileged Identity Management.

3. En Tareas, seleccione Mis roles.

![image](https://user-images.githubusercontent.com/110675810/191299821-a0f8a641-e6b4-476d-8a51-ef484fbe23af.png)

4. En Activar, seleccione Recursos de Azure.

![image](https://user-images.githubusercontent.com/110675810/191299931-c60208ef-111f-45e4-863d-d82383722934.png)

5. En la pestaña Roles activos, observe que no tiene ningún rol asignado.

![image](https://user-images.githubusercontent.com/110675810/191300093-15b40333-b496-453f-95ef-efc7c49deb54.png)

6. En la pestaña Roles elegibles, desplácese a la derecha y seleccione Activar el rol.

![image](https://user-images.githubusercontent.com/110675810/191300878-43657cca-0487-4fc1-ac44-a3b456a4815e.png)

7. Observe la Hora de inicio y la Duración.

8. Indique un motivo para la activación. Por ejemplo, "Necesidad de agregar una NIC".

9. Haga clic en Activar.

10. El Estado de activación debe mostrar que se han completado todas las fases de activación.

11. Use el vínculo para Cerrar sesión.

12. Debe cerrar la sesión y volver a iniciarla para empezar a usar el rol recién activado.

### PRUEBA DE ACCESO AL ROL

En esta tarea, vamos a asegurarnos de que el rol se ha asignado.

1. Inicie sesión en el portal como AZ500User1.

2. Busque y seleccione Azure AD Privileged Identity Management.

![image](https://user-images.githubusercontent.com/110675810/191302128-b0264a18-649f-4889-9990-6ccbf0202724.png)

3. En Activar, seleccione Recursos de Azure.

![image](https://user-images.githubusercontent.com/110675810/191303033-79e15c5c-8f7a-4471-add9-916beb1ac79d.png)

4. Seleccione la pestaña Roles activos y compruebe que el rol Colaborador de la máquina virtual se haya activado.

![image](https://user-images.githubusercontent.com/110675810/191303188-0602fc6b-01ab-400a-b509-4f523efda2d0.png)

5. Cierre la sesión en el portal.

![image](https://user-images.githubusercontent.com/110675810/191303307-6cdbf807-cb5e-4549-9130-d719bc541e39.png)

6. Inicie sesión en el portal con una cuenta de administrador global.

7. Busque y seleccione Azure Active Directory.

![image](https://user-images.githubusercontent.com/110675810/191303698-1296e8a6-4248-437a-9ece-958cabed8aa6.png)

8. En Administrar, haga clic en Usuarios.

9. Seleccione AZ500User1.

![image](https://user-images.githubusercontent.com/110675810/191303913-be24418d-bdb2-4c1c-85f9-7e5cb0ce11ae.png)

10. En Administrar, haga clic en Roles asignados.

11. Compruebe que no aparece ningún rol.

![image](https://user-images.githubusercontent.com/110675810/191304122-35be6468-8f86-4efb-b88a-b57c41db9011.png)

12. En Administrar, seleccione Asignaciones de roles de Azure.

13. Compruebe que aparezca el rol Colaborador de la máquina virtual.

![image](https://user-images.githubusercontent.com/110675810/191304700-8228e060-f731-4177-97f4-940883ad2f33.png)
