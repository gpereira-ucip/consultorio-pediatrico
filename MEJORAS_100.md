# Consultorio Pediátrico — 100 mejoras

Lista de trabajo de la tarea diaria. Se resuelven **en orden**, todas las que se puedan por día.
Estados: `[ ]` pendiente · `[x]` hecho (con versión y fecha) · `[~]` en curso (anotar qué falta) · `[!]` bloqueado (anotar por qué: falta fuente oficial, necesita decisión de Gonzalo, etc.).
Todo contenido clínico nuevo va con fuente oficial (SAP, MSAL, Garrahan, OMS) y queda en «Pendiente de revisión médica» de PROYECTO.md.

## A. Velocidad y flujo de trabajo
1. [x] (v1.4.1, 09/11) Arreglar el desborde horizontal en celular (≈390 px): selector Consulta/Control/Alta y barra inferior.
2. [x] (v1.4.2, 09/11) Atajos de teclado: Alt+1…6 para pestañas, Ctrl+K buscar cuadro, Esc cerrar ventanas; ayuda de atajos con «?».
3. [x] (v1.4.3, 09/11) Buscador rápido de intercurrencias: escribir «otitis» y elegir, en lugar de la lista larga.
4. [x] (v1.4.4, 09/11) Cuadros más usados primero en el selector (contador local, sin datos de pacientes).
5. [x] (v1.4.5, 09/11) Copias parciales: «Copiar solo examen físico», «Copiar solo plan/conducta», «Copiar solo antropometría».
6. [x] (v1.4.6, 09/11) Formato del texto desde la barra inferior: con títulos / texto corrido / con viñetas.
7. [x] (v1.4.7, 09/11) Deshacer «Nuevo paciente» durante 30 segundos.
8. [!] Recuperar el borrador si se cierra la pestaña sin querer (solo en la sesión, sin nombre ni DNI). Necesita OK de Gonzalo, porque guarda datos clínicos de forma temporal.
9. [x] (v1.4.8, 09/11) Edad corregida para prematuros (hasta los 2 años), aplicada a hitos y percentilos, con aviso en el texto.
10. [x] (v1.4.9, 09/11) Validación de datos: avisar valores imposibles o improbables (peso, talla, T°, FC, FR, SatO₂) para la edad.
11. [!] Signos vitales con rango normal por edad y marca de color si están fuera de rango (fuente oficial). Bloqueado 09/11: no encontré una tabla oficial argentina (SAP, MSAL, Garrahan) de FC y FR normales por edad; la guía MSAL de IRA (2011) solo trae el Tal y fiebre ≥38 °C, y el consenso SAP de shock séptico (2019) solo FC. Necesita que Gonzalo elija la referencia (p. ej., PALS/AHA 2020, «Criterios de atención» del Garrahan o la tabla que usa) para cargarla.
12. [!] Frase automática de signos vitales en la evolución («taquicárdico para la edad», «febril») según rangos. Bloqueado 09/11: depende de los rangos del ítem 11. «febril / subfebril / afebril» ya sale en el texto desde v1.0.0 (T ≥38 / ≥37,5).
13. [x] (v1.4.10, 09/11) Modo compacto para pantallas chicas o ventana partida al lado del sistema de turnos.
14. [x] (v1.4.11, 09/11) Tamaño de letra ajustable (A−/A+) guardado en Ajustes.
15. [x] (v1.4.12, 09/11) Pantalla de inicio rápida: tres botones grandes (Control · Intercurrencia · Apto) al abrir la app.

## B. Control de salud
16. [x] (v1.4.13, 09/11) Impresión diagnóstica automática y editable («Niño sano. Crecimiento y desarrollo acordes a edad»).
17. [x] (v1.4.14, 09/11) Alertas de crecimiento en pantalla y frase sugerida: Pc <3 o >97, cruce de 2 líneas, IMC con sobrepeso u obesidad (OMS).
18. [x] (v1.4.15, 09/11) Recién nacido: % de descenso de peso respecto del nacimiento y alerta si no recuperó el peso a los 10-15 días.
19. [x] (v1.4.16, 09/11) Chips rápidos de alimentación por edad (tomas, volumen, semisólidos, agua, jugos, ultraprocesados).
20. [x] (v1.4.17, 09/11) Chips de sueño, esfínteres, pantallas y lectura según la edad.
21. [x] (v1.4.18, 09/11) Pesquisas por edad del MSAL 2018 (OEA, reflejo rojo, caderas, anemia, visión, audición, PA desde los 3 años, lípidos) con estado hecho/pendiente.
22. [!] M-CHAT-R/F a los 18-24 meses con puntaje y conducta (verificar condiciones de uso de la versión en español). Bloqueado 09/11: el M-CHAT-R/F (© Robins, Fein y Barton) no es de código abierto; su documento oficial (mchatscreen.com, rev. marzo 2025) pide permiso a Diana L. Robins para cualquier uso electrónico o en software (un consultorio puede cargar las preguntas en su propia HC, pero no distribuirlas). Necesita que Gonzalo decida si pide el permiso (y qué traducción oficial al español usar).
23. [!] (parcial v1.4.19, 09/11) Pesquisa de depresión puerperal (Escala de Edimburgo) en los controles del primer año. Hecho: campo de puntaje total 0-30 que sale en el texto sin interpretación. Falta: los 10 ítems y el punto de corte, que requieren la versión oficial en español validada (no la encontré en MSAL/SAP, segunda búsqueda 09/11 tarde sin resultado; si Gonzalo usa una, que la pase y se completa).
24. [x] (v1.4.20, 09/11) Salud bucal por edad: flúor, primera consulta odontológica, riesgo de caries.
25. [x] (v1.4.21, 09/11) Prevención de lesiones por edad ampliada con la SAP, como chips.
26. [x] (v1.4.22, 09/11) Adolescencia: guía HEEADSSS con chips (lo confidencial no se guarda).
27. [!] (parcial v1.4.23, 09/11) Tanner con selector visual y edad esperable de cada estadio. Hecho: selector de un clic M/G (según sexo) y VP 1-5 en Apto y en el control de adolescencia (completa «Tanner M_ VP_» del examen físico). Falta: la edad esperable de cada estadio — no encontré tablas oficiales argentinas (SAP/Lejarraga) con media y P3-P97 por estadio; conseguirlas para cargarlas. Sin dibujos (decisión: solo botones con texto).
28. [x] (v1.4.24, 09/11) Plantilla de seguimiento del prematuro (ROP, OEA, edad corregida, suplementos, vacunas).
29. [x] (v1.4.25, 10/11) Plantilla de control en síndrome de Down (guía SAP) con estudios por edad. Fuente: Kaminker y Armando, Arch Argent Pediatr 2008 (SAP). Sin curvas de SD (ítem 54).
30. [x] (v1.4.26, 10/11) Certificado de salud escolar / libreta de salud listo para copiar (en Apto físico). Cada jurisdicción tiene su formulario: el texto es para transcribir.

## C. Intercurrencias
31. [x] (v1.4.27, 10/11) Nuevos cuadros (1): dermatitis atópica, cólicos del lactante, reflujo, prúrigo/picaduras.
32. [x] (v1.4.28, 10/11) Nuevos cuadros (2): sinusitis, adenitis, epistaxis, cuerpo extraño (nariz/oído), intoxicaciones (teléfonos del MSAL: Posadas, Gutiérrez, Sor María Ludovica).
33. [!] (parcial v1.4.29, 10/11) Nuevos cuadros (3): pediculosis, molusco, tiña, vulvovaginitis, balanopostitis, sinequias. Hecho: pediculosis, molusco, tiña capitis, vulvovaginitis inespecífica y sinequias vulvares. Falta: balanopostitis y tiña corporis — no encontré guía SAP/MSAL/Garrahan con su tratamiento (solo fuentes extranjeras); si Gonzalo pasa la referencia que usa, se cargan.
34. [!] (parcial v1.4.30, 10/11) Nuevos cuadros (4): crisis asmática, escarlatina, mononucleosis, coqueluche, convulsión febril (consulta posterior). Hecho: crisis asmática, escarlatina, mononucleosis y coqueluche. Falta: convulsión febril — no encontré guía SAP/MSAL/Garrahan sobre convulsión febril (definición, estudios, consejos a la familia); si Gonzalo pasa la referencia que usa, se carga.
35. [!] (parcial v1.4.31, 10/11) Nuevos cuadros (5): quemaduras, mordedura de perro, cojera/dolor de miembros, cefalea, síncope. Hecho: mordedura de perro y síncope. Falta: quemaduras (solo encontré primeros auxilios del Garrahan, sin manejo ambulatorio ni criterios de derivación), cojera/dolor de miembros y cefalea — sin guía SAP/MSAL/Garrahan; si Gonzalo pasa las referencias que usa, se cargan.
36. [x] (v1.4.32, 10/11) Fiebre: chips de máximo, días, horario y respuesta a antitérmicos.
37. [~] (v1.4.33, 10/11) Banderas rojas por cuadro, en pantalla (no en el texto), con fuente. Hecho: tarjeta «🚩 Banderas rojas y derivación» (objeto `ALERTA`) cargada en 19 cuadros (bql, bronco, da, colico, rge, prurigo, sinus, adenitis, epist, ce, intox, coq, mono, mord, sincope, vv, sineq, tina). Falta: cargar con fuente los cuadros originales (CVAS, rinofaringitis, faringitis, OMA, otitis externa, laringitis, NAC, GEA, dolor abdominal, constipación, ITU, conjuntivitis, exantema, urticaria, escabiosis, oxiuriasis, impétigo, celulitis, trauma, herida, TEC, SFSF, dengue, varicela, parotiditis, tortícolis, PFP, muguet, pañal, asma, escarlatina, pediculosis, molusco).
38. [~] (v1.4.33, 10/11) Criterios de derivación o internación por cuadro, en pantalla, con fuente. Hecho: misma tarjeta del ítem 37 (sección «Derivación / internación / interconsulta»), con datos en bql, bronco, da, sinus, adenitis, epist, ce, intox, mord, sincope y sineq. Falta: el resto de los cuadros, con fuente.
39. [~] (v1.4.34, 10/11) Pautas de alarma específicas por cuadro, editables, que salen en la conducta. Hecho: campo editable (`iPA`) precargado con las pautas del cuadro, que sale en la conducta y se guarda en Mis plantillas; 25 cuadros ya traen pautas específicas. Falta: cargar con fuente las pautas de los cuadros que dicen solo «Se dan pautas de alarma» (CVAS, rinofaringitis, faringitis, OMA, etc.; mientras tanto Gonzalo puede escribirlas y guardarlas como plantilla propia).
40. [x] (v1.4.35, 10/11) Dos diagnósticos en la misma consulta (ej. OMA + conjuntivitis): combinar cuadros.
41. [x] (v1.4.36, 10/11) Antecedentes con chips (asma, alergias, prematurez, cardiopatía, internaciones).
42. [x] (v1.4.37, 10/11) Alergia a penicilina tildada: ocultar o advertir los betalactámicos y sugerir la alternativa de la plantilla.
43. [x] (v1.4.38, 10/11) Peso ≥40 kg o adolescente: aviso de dosis de adulto y topes visibles.
44. [x] (v1.4.39, 11/11) Fecha de fin del tratamiento calculada («por 10 días, hasta el 19/11»).
45. [x] (v1.4.40, 11/11) Control evolutivo con chips (mejoró / igual / peor, afebril desde…, completa tratamiento).
46. [~] Hidratación: plan A/B/C de la OMS con volúmenes calculados por peso. No empezado: el 11/11 la sesión no tuvo acceso web a las fuentes (red del entorno limitada: sap.org.ar, argentina.gob.ar, who.int, etc. no resolvían). Fuente a usar: MSAL, «Plan de abordaje integral de la enfermedad diarreica aguda», Guía para el equipo de salud N.º 8 (planes A, B y C). Reintentar cuando haya acceso.
47. [~] Presentaciones comerciales frecuentes en Argentina por fármaco y redondeo práctico a ml o gotas (revisión médica). No empezado: sin acceso web el 11/11 (ver ítem 46); además conviene que Gonzalo pase la lista de presentaciones que receta. Reintentar.
48. [x] (v1.4.41, 11/11) Revisar y unificar el estilo de todas las plantillas de intercurrencia (abreviaturas, tildes, orden).

## D. Crecimiento y percentilos
49. [x] (v1.4.42, 11/11) Peso para la talla (OMS, 0-5 años). Tablas LMS oficiales (repo «anthro» de la OMS); Pc y z en encabezado, texto, tabla, curva y alertas.
50. [x] (v1.4.43, 11/11) Velocidad de crecimiento (cm/año) a partir de las mediciones previas. Solo el cálculo (sin percentilos de velocidad: no hay tablas cargadas).
51. [x] (v1.4.44, 11/11) Percentilo de presión arterial (tablas AAP 2017) por edad, sexo y talla. Ubica PAS y PAD respecto de P50/P90/P95 (1-17 años); no clasifica estadios de hipertensión (falta verificar los criterios en la guía original).
52. [!] Tablas SAP (Lejarraga) 5-19 años como alternativa a OMS 2007 (solo con valores oficiales).
53. [!] Curvas de prematuros (Intergrowth-21st o Fenton), si se consiguen los datos oficiales con licencia de uso. Bloqueado 11/11: necesita decisión de Gonzalo — (a) cuál usar (Fenton 2013 o INTERGROWTH-21st posnatal de prematuros); (b) los datos existen en paquetes de terceros (p. ej. «gigs» para INTERGROWTH-21st), pero no pude confirmar la licencia de uso de las tablas originales (sin acceso web a los sitios oficiales el 11/11).
54. [~] Curvas para síndrome de Down (SAP), si se consiguen los datos oficiales. No empezado: sin acceso web a sap.org.ar el 11/11 (ver ítem 46). Reintentar; si la SAP no publica tablas numéricas (LMS o percentilos), pasar a [!].
55. [x] (v1.4.45, 11/11) Lector de mediciones previas más tolerante (pegar «12/3 7,2kg 66cm» o el texto de la HC).
56. [x] (v1.4.46, 11/11) Imagen única con las curvas en formato A4 para pegar o imprimir.
57. [x] (v1.4.47, 11/11) Blanco genético dibujado en la curva de talla.
58. [x] (v1.4.48, 11/11) Frase automática de crecimiento («crece en el canal del Pc 50, sin cruces de líneas»).

## E. Vacunas
59. [~] Esquemas atrasados: plan de recupero con intervalos mínimos (Lineamientos MSAL). No empezado: sin acceso web a las fuentes oficiales el 11/11 (red del entorno limitada; ver «Problemas conocidos» en PROYECTO.md). Reintentar. La v1.4.49 ya lista las dosis atrasadas según el carnet tildado, sin intervalos.
60. [~] Vacunas para grupos de riesgo como recordatorio (antigripal, neumococo, meningococo B, etc.). No empezado: sin acceso web a las fuentes oficiales el 11/11 (red del entorno limitada; ver «Problemas conocidos» en PROYECTO.md). Reintentar.
61. [~] Vacuna contra el dengue según zona y edad (MSAL vigente). No empezado: sin acceso web a las fuentes oficiales el 11/11 (red del entorno limitada; ver «Problemas conocidos» en PROYECTO.md). Reintentar.
62. [x] (v1.4.49, 11/11) Tildar dosis recibidas en la tabla y calcular la próxima fecha exacta.
63. [~] Aviso de campaña antigripal según el mes del año. No empezado: sin acceso web a las fuentes oficiales el 11/11 (ver «Problemas conocidos» en PROYECTO.md). Reintentar. (Hace falta la fecha de inicio de la campaña que publica el MSAL cada año.)
64. [x] (v1.4.50, 11/11) Texto para la familia: «Próximas vacunas: … a partir del …» (para WhatsApp).
65. [~] Vacunas de convivientes y embarazadas (dTpa, antigripal, VSR) como consejo en los controles del RN. No empezado: sin acceso web a las fuentes oficiales el 11/11 (ver «Problemas conocidos» en PROYECTO.md). Reintentar.
66. [~] Contraindicaciones y precauciones frecuentes, en pantalla. No empezado: sin acceso web a las fuentes oficiales el 11/11 (ver «Problemas conocidos» en PROYECTO.md). Reintentar.

## F. Recetas, certificados e indicaciones
67. [x] (v1.4.51, 11/11) Receta de medicamentos: fármaco, presentación, dosis, frecuencia, días y cantidad de envases. En la pestaña nueva «Recetas» (Alt+7).
68. [x] (v1.4.52, 11/11) Certificado de reposo o evicción con fechas desde/hasta.
69. [x] (v1.4.53, 11/11) Certificado de apto escolar / educación física (pestaña Recetas; el certificado de salud escolar completo sigue en Apto físico).
70. [x] (v1.4.54, 11/11) Certificado de apto para natación (piel, uñas, pies).
71. [~] (v1.4.55, 11/11) Indicaciones para la familia en lenguaje simple, para copiar a WhatsApp. Hecho: tarjeta «Mensaje para la familia» en Intercurrencia que arma el mensaje con la conducta tildada (sin el cálculo en mg/kg), reposo, pautas de alarma y control. Falta: reescribir en lenguaje llano las indicaciones de cada cuadro (hoy salen con la redacción de la HC, p. ej. «Medidas higiénico-dietéticas»); necesita redacción revisada por Gonzalo o fuente para familias (SAP/MSAL), sin acceso web el 11/11.
72. [x] (v1.4.55, 11/11) Pautas de alarma para la familia por cuadro (WhatsApp). Usa las pautas de alarma del cuadro (editables); los cuadros sin pautas específicas dependen del ítem 39.
73. [ ] Hoja de alimentación complementaria por edad para la familia (fuente: MSAL/SAP).
74. [ ] Hojas para la familia: sueño seguro, lactancia, prevención de accidentes por edad.
75. [ ] Interconsultas y derivaciones redactadas (cardiología, ORL, oftalmología, traumatología…).
76. [ ] Pedido de estudios redactado (laboratorio, Rx, ecografía) con diagnóstico presuntivo.

## G. Scores y calculadoras
77. [ ] Pulmonary Score (Guía SAP de asma; conseguir la tabla oficial).
78. [ ] Score de Westley (laringitis) con texto para la HC.
79. [ ] Escala de Gorelick (deshidratación).
80. [ ] Glasgow pediátrico.
81. [ ] Holliday-Segar y déficit de líquidos.
82. [ ] Superficie corporal (Mosteller).
83. [ ] Calculadora de dosis libre (mg/kg → ml según concentración, con tope).
84. [ ] Score de McIsaac para faringitis (en pantalla, apoya la decisión del test).
85. [ ] Fiebre sin foco en menores de 3 meses: criterios de bajo riesgo como recordatorio en pantalla.
86. [ ] Conversor de unidades (lb↔kg, °F↔°C, pulgadas↔cm).

## H. Diseño y experiencia
87. [ ] Íconos propios, coherentes con los logos, en lugar de emojis.
88. [ ] Microanimaciones suaves al copiar, abrir tarjetas y cambiar de pestaña.
89. [ ] Vista previa con resaltado de lo agregado o modificado respecto de la plantilla.
90. [ ] Modo oscuro opcional para guardias nocturnas.
91. [ ] Diseño de impresión (Ctrl+P) limpio para indicaciones, recetas y curvas.
92. [ ] Accesibilidad: foco visible, navegación completa con Tab, etiquetas ARIA, contraste AA.
93. [ ] Pantalla «Novedades» con lo que cambió en cada versión.
94. [ ] Tarjeta del paciente más compacta cuando se hace scroll (encabezado pegajoso con edad, sexo y peso).

## I. Calidad, respaldo y confianza
95. [ ] Sección «Fuentes y actualización» con fecha de cada referencia.
96. [ ] Autodiagnóstico interno (botón en Ajustes) que verifique todas las plantillas y cálculos.
97. [ ] Exportar e importar toda la configuración (frases, plantillas, ajustes) en un solo archivo.
98. [!] Adaptar el texto al sistema de HC que usa Gonzalo (campos separados para pegar uno por uno). Necesita que Gonzalo diga qué campos tiene su sistema.
99. [ ] Revisión ortográfica y de estilo de todo el contenido.
100. [ ] Optimizar peso y velocidad del archivo (fuentes, imágenes, código) sin perder funciones.

## Ya hechas antes de esta lista
- Mis frases (v1.2.0) · Mis plantillas de intercurrencia (v1.3.0) · Puntaje de Tal (v1.4.0).
