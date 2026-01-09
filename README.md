# Gestionale Bandi di Gara

## 1. Introduzione generale

Questo progetto nasce come elaborato di esame universitario nell’ambito dei corsi di **Object-Oriented Programming** e **Back-End Programming**.  
L’obiettivo non è soltanto realizzare un’applicazione funzionante, ma costruire una base software **coerente, verificabile e tracciabile**, in cui ogni funzionalità implementata sia riconducibile a requisiti, use case e test formalizzati.

La gestione dei **bandi di gara** è stata scelta come dominio applicativo perché reale, normativamente vincolato e sufficientemente complesso da giustificare:
- modellazione del dominio rigorosa,
- applicazione di pattern OOP,
- separazione architetturale multilivello,
- verificabilità tramite test.

---

## 2. Architettura generale

Il progetto adotta un’architettura multilayer ispirata a **Clean Architecture** e **DDD**, con dipendenze orientate verso il dominio.

**Caratteristiche principali**
- Monorepo Maven multi-module
- Dominio Java puro, privo di dipendenze infrastrutturali
- Application layer come orchestratore dei casi d’uso
- Delivery multipla: CLI, REST, SOAP
- Persistenza differenziata per contesto didattico

**Moduli**
```
gestionale-bandi-domain
gestionale-bandi-application
gestionale-bandi-cli
gestionale-bandi-infrastructure
gestionale-bandi-api-rest
```
.
