# Configuración de Azure AD Privileged Identity Management
## Tarea 6: Azure AD PIM para roles

En esta tarea, vamos a configurar las opciones de activación de PIM, agregar Administrador de facturación como un rol de PIM, activar el rol y probar la activación.

CONFIGURACION DE PIM

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


CONFIGURACION DE PIM PARA LOS ROLES 

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


PRUEBA DE ACCESO AL ROL

En esta tarea, pruebe el rol Administrador de facturación.

1. Inicie sesión en el portal como AZ500User1.

![image](https://user-images.githubusercontent.com/110675810/189481860-6bdf2ca8-f53c-435a-9f95-b6f8bd8a73ff.png)

![image](https://user-images.githubusercontent.com/110675810/189482095-69443df7-8ad4-447d-b4f1-24b776346fa1.png)

2. Busque y seleccione Azure AD Privileged Identity Management.

3. En Activar, seleccione Roles de Azure AD.

![image](https://user-images.githubusercontent.com/110675810/189482209-b456c3c0-46d8-42ee-8b97-9c689a84a60e.png)

![image](https://user-images.githubusercontent.com/110675810/189482252-4e1ae2c7-1103-4855-8176-cf478823734f.png)

4. Seleccione la pestaña Roles activos y compruebe que el rol Administrador de facturación se haya activado.

5. El rol debería aparecer ahora como Activado.

![image](https://user-images.githubusercontent.com/110675810/189482277-60219f16-5aee-463a-914a-5cc370cb03ba.png)

6. Observe que existe la opción de Desactivar el rol.

Nota: Se puede cancelar solicitud

![image](https://user-images.githubusercontent.com/110675810/189482489-32610a43-b12c-4bfb-9b05-3da293e3a043.png)

