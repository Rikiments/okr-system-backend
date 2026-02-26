# 🎯 API REST para Gestão de OKRs

> Sistema backend para gerenciamento e acompanhamento de Objetivos e Resultados Chave (OKRs).

## 📖 Sobre o Projeto
Este projeto é uma API RESTful desenvolvida em **Java com Spring Boot**, projetada para auxiliar no gerenciamento de OKRs (Objectives and Key Results). 

O grande diferencial do sistema é a sua **lógica de cálculo automático**: o progresso de um Objetivo é atualizado dinamicamente com base na conclusão de suas Iniciativas e Tarefas, criando um efeito cascata que mantém os dados sempre sincronizados sem necessidade de intervenção manual.

## 🚀 Tecnologias Utilizadas

* **Java 17**
* **Spring Boot 3**
* **Spring Data JPA (Hibernate)**
* **PostgreSQL** (Hospedado no Supabase)
* **Lombok** (Para redução de boilerplate code)
* **Maven** (Gerenciamento de dependências)

## ✨ Destaques e Funcionalidades

* **Cálculo em Cascata:** A conclusão de uma *Task* atualiza a *Iniciativa*, que atualiza o *Key Result*, que por fim atualiza a porcentagem do *Objetivo*.
* **Tratamento de JSON:** Implementação correta de `@JsonManagedReference` e `@JsonBackReference` para evitar loops infinitos em relacionamentos bidirecionais.
* **Arquitetura em Camadas:** Código organizado em Controllers, Services e Repositories.
* **CRUD Completo:** Operações de criação, leitura, atualização e exclusão para todas as entidades.
* **Clean Code:** Uso de DTOs (Data Transfer Objects) e injeção de dependências.
