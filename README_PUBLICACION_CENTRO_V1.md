# Centro Informe Fin de Turno v1.0 RC — Multiusuario

## Objetivo de esta versión
Permitir que el Centro sea usado por más de un computador:

- Mario administra el Plan Semanal: carga Excel/SAP, procesa y publica.
- Supervisora / usuario de turno solo conecta al backend y presiona **Actualizar informes**.
- El Centro recupera automáticamente el **Plan Activo** desde el backend antes de consultar registros.

## Archivo para publicar
Renombrar este archivo como `index.html` en el repositorio GitHub Pages:

```text
centro_informes_turno_v1_0_RC_multiusuario.html
```

## Flujo esperado

### Mario / administrador del plan
1. Abrir Centro.
2. Conectar backend.
3. Cargar Plan Semanal inicial / siguiente.
4. Procesar plan.
5. Revisar conflictos.
6. Publicar Plan Semanal.
7. Confirmar: `✓ Plan publicado y verificado`.

### Supervisora / usuario de turno
1. Abrir Centro desde la URL publicada.
2. Configurar backend una sola vez.
3. Presionar **Guardar y probar**.
4. El Centro carga el Plan Activo desde backend.
5. Presionar **Actualizar informes**.
6. Generar informe cuando corresponda.

## Prueba de aceptación antes de publicar

1. Publicar un plan desde el PC de Mario.
2. Abrir el Centro en otro navegador o modo incógnito.
3. Configurar backend.
4. Confirmar que aparece `✓ Plan Activo cargado` sin cargar Excel.
5. Presionar **Actualizar informes**.
6. Confirmar que se ven OT ejecutadas / pendientes / reprogramadas.
7. Abrir pestaña INFORME y actualizar vista previa.
8. Confirmar fotos PM03 y registros del turno.

## Repositorio sugerido

```text
apps-mtto-ant/centro-informes-turno
```

URL esperada:

```text
https://apps-mtto-ant.github.io/centro-informes-turno/
```
