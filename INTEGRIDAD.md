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
  20/11. Las horas consignadas no son horas reales de ejecución.
- Según la explicación del equipo, quien fijó esas fechas fue el propio
  Anthony; los demás integrantes no lo sabían. Anthony tiene poco conocimiento
  de Git y estaba usando ayuda de una herramienta de inteligencia artificial
  para trabajar en el repositorio, y esa ayuda produjo ese resultado. Se
  desconoce la hora real en que realizó ese trabajo.
- Como consecuencia, el orden de fechas de autor no coincide con el orden
  topológico de los commits. No se realizará otra reescritura para disimularlo
  ni para trasladar la responsabilidad a otros integrantes.

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
- No modifican la grabación original ni **se presentan como consentimiento
  obtenido antes de las entrevistas**. El ítem de depósito en repositorio
  abierto de `ENTR-03` sigue sin respuesta y no se completó.

## 5. Grabaciones

- EV-10 a EV-13 registran nombre de archivo, fecha, duración y SHA-256 reales
  de los cuatro videos.
- Las entrevistas fueron realizadas por el líder del equipo. `ENTR-02` se
  realizó con la cocinera y `ENTR-03` con la auxiliar de cocina.
- Dos de esos archivos son byte-a-byte idénticos a grabaciones tituladas como
  «Reunión con JEANPIERRE ROBINSON ESPINOZA» en OneDrive. El título usa el
  nombre del líder porque fue quien organizó y grabó la sesión; no identifica
  a la persona entrevistada.
- La fecha real de esas dos sesiones es la de los archivos originales:
  `ENTR-02` es del 18/11/2026 y `ENTR-03` es del 21/11/2026. El manifiesto
  había consignado 20/11 para las cuatro sesiones; ese dato se corrigió para
  estas dos. Los archivos privados se renombraron para que su nombre coincida
  con la fecha real. Su contenido y sus huellas SHA-256 no cambiaron.
- Según lo informado por el equipo, `ENTR-01` se realizó el miércoles 18/11,
  `ENTR-02` el 18/11, `ENTR-03` el 21/11 y `ENTR-04` el 20/11. El manifiesto
  había declarado 20/11 para las cuatro; se corrigió ese dato en `ENTR-01`,
  `ENTR-02` y `ENTR-03`. Los archivos de video se renombraron para que su
  nombre coincida con la fecha informada; su contenido y sus huellas SHA-256
  no cambiaron.

## 6. Verificación técnica

- Clon limpio del estado publicado compilado con
  `pdflatex → biber → pdflatex ×2`.
- Resultado: 19 páginas, pie `Página N de 19`, 0 `??`, 0 `Overfull \hbox`,
  0 `Overfull \vbox` y 0 referencias sin resolver.
