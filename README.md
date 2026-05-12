# Proxy

## Descripció de la pràctica
Aquesta pràctica consisteix en la configuració i validació d’un sistema de filtratge web mitjançant l’ús de llistes negres, filtres per categories, bloqueig de dominis i URLs específiques, filtratge per paraules clau i control horari de navegació.

L’objectiu principal és implementar una configuració funcional i correcta del proxy de filtratge, demostrant el seu funcionament amb proves i evidències.

---

# Apartats implementats

## 1. Instal·lació de llistes negres
S’han instal·lat les llistes negres de la Universitat de Toulouse i s’ha configurat l’actualització automàtica periòdica.

### Tasques realitzades
- Instal·lació de les llistes negres.
- Configuració del repositori.
- Programació de l’actualització automàtica.
- Verificació de la compilació correcta de les llistes.

### Resultat
El sistema aplica correctament les llistes negres i manté la base de dades actualitzada.

---

## 2. Filtrat per categories (Bank i Radio)
S’ha configurat el bloqueig de les categories:
- **Bank**
- **Radio**

### Verificació
S’ha comprovat el funcionament correcte del filtratge accedint als llocs de prova:
- `ing.es`
- `ah.fm`

### Resultat
Les pàgines incloses en aquestes categories queden bloquejades correctament pel proxy.

---

## 3. Filtrat de dominis i URLs
S’ha configurat una “Llista Negra personalitzada” per bloquejar dominis i URLs específiques.

### Dominis bloquejats
- `elnacional.capgros.cat`
- `tecnocampus.cat`

### Configuració addicional
També s’ha implementat el bloqueig selectiu de URLs sense afectar la resta del domini.

### Resultat
El filtratge funciona correctament tant a nivell de domini com de URL específica.

---

## 4. Filtrat de paraules i exclusions (Anime)
S’ha configurat un filtre de paraules per bloquejar el terme:
- `anime`

### Excepció configurada
S’ha afegit una whitelist per permetre l’accés a:
- `animenewsnetwork.com`

### Resultat
El sistema bloqueja correctament el contingut relacionat amb “anime”, excepte el domini autoritzat.

---

## 5. Control horari
S’ha implementat una restricció horària de navegació mitjançant el mòdul de filtratge.

### Configuració
- Creació de regles temporals.
- Aplicació de restriccions segons horaris definits.
- Assignació a categories i hosts específics.

### Resultat
Les restriccions s’apliquen correctament segons la planificació configurada.

---

# Evidències
La pràctica inclou captures de pantalla i comprovacions de:
- Funcionament del proxy.
- Bloqueig de categories.
- Bloqueig de dominis i URLs.
- Filtrat per paraules.
- Funcionament de les excepcions.
- Aplicació de restriccions horàries.

---

# Conclusions
La configuració del sistema de filtratge s’ha implementat correctament complint els requisits de la pràctica. El proxy aplica les polítiques de seguretat definides i permet gestionar l’accés a continguts web de manera eficient i controlada.

![Enllaç de la practica](practica.md)
