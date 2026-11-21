# Nota de integridad — TA-PFC-E1

Esta nota se registra voluntariamente para explicar decisiones de historial,
autoría y evidencias. No sustituye la explicación que debe darse al docente.

## 1. Origen del nombre de la organización

- `Anaranjoa-UX` era el nombre de la cuenta de GitHub de un integrante del
  equipo, **no** el nombre del restaurante.
- Al detectarse el error se corrigió ese texto en archivos y mensajes de commit
  a `El Balcón Restaurant, Quevedo, Los Ríos`.
- Esa corrección implicó reescribir el historial y hacer un force-push. Los
  momentos reales en que se hicieron los push y los force-push constan en los
  registros del servidor de GitHub y no se han modificado.

## 2. Fechas de autoría de los commits de Anthony

- Los commits `3deea7b` y `b5ed20a`, con autoría de Naranjo Alfonzo Anthony
  Alexander, tienen **fechas de autor fijadas manualmente** para el 19/11 y
  20/11, tomadas como referencia de los ZIP de trabajo fechados esos días.
  Las horas consignadas no son horas reales de ejecución.
- Como consecuencia, el orden de fechas de autor no coincide con el orden
  topológico de los commits. No se realizará otra reescritura para disimularlo.

## 3. Evidencias pendientes

- EV-01 (carta de aceptación firmada) se recibió el 21/11 como copia digital
  de un documento con fecha impresa 18/11. Se guardó en la carpeta privada
  `@uteq.edu.ec` y solo se publica su nombre de archivo, fecha y SHA-256 en
  `MANIFIESTO.md`; el original contiene nombre, firma y cargo y no se sube al
  repositorio.
- EV-02 (registro del primer contacto) se diligenció el 21/11 con base en la
  información reportada por el equipo sobre el contacto del 18/11 a las 1:20
  pm, por medio digital, atendido por la administradora (`AD-01`). Es por tanto
  un registro documentado después del hecho, no un acta simultánea; se guarda
  en `@uteq.edu.ec` y en el repositorio solo se publican su nombre de archivo,
  fecha y SHA-256. No se inventaron nombres ni datos de contacto.

## 4. Adendums de consentimiento

- EV-07, EV-08 y EV-09 se emitieron el 21/11 para documentar ítems que la
  herramienta de transcripción omitió en `ENTR-03`, `ENTR-01` y `ENTR-04`.
- No cambian la fecha de las entrevistas (20/11) y **no se presentan como
  consentimiento obtenido después de las entrevistas**. El ítem de depósito en
  repositorio abierto de `ENTR-03` sigue sin respuesta y no se completó.

## 5. Grabaciones

- EV-10 a EV-13 registran nombre de archivo, fecha declarada, duración y
  SHA-256 reales de los cuatro videos.
- Dos de esos archivos son byte-a-byte idénticos a grabaciones tituladas como
  «Reunión con JEANPIERRE ROBINSON ESPINOZA» en OneDrive (18/11 y 21/11). Su
  condición de entrevistas de campo debe aclararse con evidencia o declararse
  ante el docente. No se ha alterado su contenido ni sus huellas.

## 6. Verificación técnica

- Clon limpio del estado `4800545` compilado con
  `pdflatex → biber → pdflatex ×2`.
- Resultado: 19 páginas, pie `Página N de 19`, 0 `??`, 0 `Overfull \hbox`,
  0 `Overfull \vbox` y 0 referencias sin resolver.
