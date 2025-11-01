
---
title: "OSWP: Trucos and Consejos para Pwnear todas las Redes!"
summary: "Recientemente obtuve la certificación OSWP y en este post te cuento cómo me preparé y qué aprendí de toda la experiencia!"
categories: ["Post","Blog",]
tags: ["certification experience"]
#externalUrl: ""
#showSummary: true
draft: false
date: 2025-11-01

---

## **Aprobé el OSWP!**

Me enorgullece anunciar que he obtenido la certificación **Offensive Wireless Professional (OSWP)**. Esta certificación proporciona un excelente conocimiento complementario al OSCP, para que añadas nuevas habilidades a tú cinturón de pentester. Las redes Wi-Fi están por todas partes y son un excelente entry point a tener en cuenta.

![OSWP1](/img/oswp/oswp1.png)

La verdad que ha sido una experiencia buena y enriquecedora. En esta post hablaremos sobre mi trayectoria en el Hacking WiFi, así como algunos consejos y trucos para aprender lo necesario para obtener esta certificación.

## La experiencia PEN-210

>PEN-210 (Ataques inalámbricos) introduce los fundamentos de la seguridad de redes inalámbricas, explorando vulnerabilidades comunes y técnicas de explotación. El curso prepara a los alumnos en habilidades relacionadas con los diferentes tipos y arquitecturas de redes Wi-Fi, el reconocimiento inalámbrico y la explotación de vulnerabilidades en WPS. 

Cuando estaba estudiando para el OSCP desarrollé una excelente metodología para aprender cualquier cosa, relacionada o no con el hacking, basada en el Note Taking con Obsidian. En mi opinión, contar con una metodología buena y fiable es el paso más importante, así que tenlo presente desde el primer momento al empezar a estudiar la certi. Algún día escribiré un post sobre mi metodología... jeje

Toma buenos apuntes y cheat sheets que te permitan avanzar más rápido y perder el menor tiempo posible. Además, es aconsejable saber diferentes métodos para realizar el mismo ataque, ya que a veces herramientas diferentes dan resultados diferentes.

- - -

## Estructura y preparación del examen

Aunque no puedo entrar en detalles concretos sobre el examen, puedo confirmar que el curso incluye todo lo necesario para aprobar. Sin embargo, tras completar el material, me pareció poca cosa. Fue entonces cuando descubrí WiFiChallenge Labs. Agradecer a [r4ulcl](https://github.com/r4ulcl) por crear este magnífico recurso.

Aquí tenéis el enlace a [WiFiChallenge Lab](https://lab.wifichallenge.com/) por si queréis echarle un vistazo.

![OSWP2](/img/oswp/oswp2.png)

Para practicar para el OSWP hay que buscarse un poco la vida, ya que necesitas una antena WiFi que se pueda poner en modo monitor y un Punto de Acceso que permita configurar los distintos entornos del examen. Aquí es donde el laboratorio WifiChallenge resulta muy útil, ya que permite probar todo en una máquina virtual sin necesidad de gastar más dinero.

Pero la verdad, si te lo puedes permitir, te recomiendo encarecidamente que configures tus propios entornos de laboratorio con equipo real. Si te mola el cacharreo como a mi, te va a gustar la experiencia.

En cuanto a la preparación, el contenido de OffSec me pareció demasiado conciso. Sentí que solo te prepara para el examen, pero no para el mundo real. Por eso recomiendo muy mucho practicar con WifiChallenge, pues vas a aparender mucho más. De nuevo, esto no es necesario para aprobar el examen, pero, al fin y al cabo, estamos aquí para aprender, no solo para aprobar certs.

Tuve la misma sensación con el curso PEN-200 para el OSCP. Me preparé el examen OSCP con el contenido del CPTS de HackTheBox, un poco overkill lo mismo, pero siempre es útil saber de más.

Por lo tanto, en mi opinión, intenta resolver todos los challenges que puedas del WifiChallenge, incluso si no forman parte del temario de PEN-210. Esto te dará una visión global más completa de las redes inalámbricas y te permitirá comprenderlas mejor.

- - -

## Día del examen. ¿Cómo fue?

Para el examen, tienes 4 horas para completar la parte técnica y 24 horas para entregar el informe. Me llevó unas 4 horas completar todo, incluyendo el informe, con las 3 flags, así que da tiempo de sobra.

Para aprobar, debes obtener las flags de al menos dos de las tres redes. Para leer una flag, primero necesitas la contraseña del punto de acceso (AP), luego conectarte a la red y tirar un `curl` para acceder al servidor web que la aloja.

Para atacar cada red necesitas conectarte por SSH a un Kali y atacar desde allí. También te dan permiso para usar RDP/VNC para tener una GUI, pero en mi experiencia iba muy lento, así que me limité a la consola.

El examen fue tal como lo esperaba. Probablemente sea el examen OffSec más directo, pero no te confíes demasiado y asegúrate de comprender bien los conceptos antes de presentarte. Tuve algunos problemas de conectividad y tuve que reiniciar el examen varias veces, pero no fue nada grave.

No te preocupes demasiado por el informe. Con que puedas explicar los ataques, hacer capturas de pantalla de los output y enviar tanto las contraseñas de los puntos de acceso como las flags asociadas, apruebas sin problema.

### Nota importante

> NO SE PERMITEN herramientas automatizadas

Si usas WiFi-Challenge Labs como entorno de práctica, asegúrate de aprender a realizar los ataques manualmente y no solo con herramientas como `eaphammer`, `eapbuster`, `wifite`, etc.

Además, asegúrate de saber usar tanto  Wireshark como Tshark, ya que, como dije antes, la interfaz gráfica va de culo.

## Experiencia general. ¿Vale la pena?

La verdad que la experiencia me ha gustado bastante. Pero, de nuevo, la experiencia general fue buena incluyendo, por supuesto, los laboratorios de WiFiChallenge. La experiencia del researching, aprender, trastear con entornos reales y practicar en entornos virtuales ha estado bastante chulo.

Por otro lado, este curso no es para quienes no tienen curiosidad ni ganas de investigar por su cuenta. Si esperas obtener todo el conocimiento en el PEN-210, probablemente este curso no sea para ti.

Estoy bastante seguro de que esto aplica a la mayoría de las certificaciones, pero siempre recomiendo ir más allá de lo requerido. Creo que buscarse la vida es la mejor manera de aprender.

Es importante mencionar que obtuve el voucher del OSWP al adquirir el paquete LearnOne con el  OSCP, que da acceso a PEN-103, PEN-200 y PEN-210 (KLCP, OSCP y OSWP, respectivamente). No recomiendo comprar el curso por separado, ya que WiFi-Challenge también ofrece sus propias certificaciones a menos de la mitad de precio, y de todas formas vas a estudiar con el WiFi-Challenge para estudiar, jaja.

Así que, una vez más, muchas gracias a [r4ulcl](https://github.com/r4ulcl) por este increíble recurso y gracias a todos por leer.

Si tienes alguna pregunta, pueden contactarme a través de mis redes sociales, como [LinkedIn](https://www.linkedin.com/in/marcosgarciaarcos/) o Discord (@s3ntinl).

Venga, nos vemos!

