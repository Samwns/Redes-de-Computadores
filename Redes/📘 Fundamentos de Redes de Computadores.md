# 📘 Fundamentos de Redes de Computadores

<p align="center">
  <img src="https://media1.tenor.com/m/-oX6GkEkoWcAAAAd/lain.gif" width="360" />
</p>

Este documento cobre os **fundamentos essenciais** do estudo de **Redes de Computadores**.
Aqui está **toda a base teórica e prática mínima**, explicada em profundidade, necessária para compreender qualquer outro assunto relacionado a:

* Segurança da Informação
* Ethical Hacking
* Servidores
* Jogos online
* Sistemas distribuídos

Nada neste arquivo é avançado — mas **tudo é fundamental**.

---

## 🧭 Visão Geral dos Fundamentos de Redes

A FASE 1 responde a uma única pergunta:

> **Como dois computadores conseguem se encontrar, se identificar e trocar dados?**

Para isso, abordamos:

* Identidade (IP)
* Localização (rede)
* Comunicação (protocolos)
* Serviços (portas)
* Tradução de nomes (DNS)

---

## 📑 Sumário

1. O que é uma rede
2. Dispositivos em uma rede
3. Tipos de rede
4. Endereçamento IP (IPv4)
5. Máscara de rede e CIDR
6. Gateway padrão
7. Portas e serviços
8. Protocolos de transporte
9. DNS em profundidade
10. Fluxo completo de comunicação
11. Erros comuns e diagnósticos iniciais

---

## 1️⃣ O que é uma rede

Uma **rede de computadores** é um sistema que permite que dois ou mais dispositivos **troquem dados** através de um meio físico ou lógico, seguindo regras bem definidas.

Sem regras, os dados existem — mas não são compreendidos.

Essas regras são chamadas de **protocolos**.

---

## 2️⃣ Dispositivos em uma rede

### Dispositivos finais

* Computadores
* Celulares
* Servidores
* Consoles

São os dispositivos que **geram e consomem dados**.

### Dispositivos intermediários

* Roteadores
* Switches
* Modems

São responsáveis por **encaminhar**, **organizar** e **direcionar** os dados.

---

## 3️⃣ Tipos de rede

### LAN — Local Area Network

* Rede restrita a uma área pequena
* Alta velocidade
* Baixa latência

Exemplos:

* Casa
* Escola
* Empresa

### WAN — Wide Area Network

* Conecta várias LANs
* Maior latência
* Infraestrutura de terceiros

Exemplo:

* Internet

---

## 4️⃣ Endereçamento IP (IPv4)

O **IP** é o identificador lógico de um dispositivo na rede.

Formato:

```
X.X.X.X
```

Cada bloco representa **8 bits** (1 byte).

Valor possível por bloco:

```
0 a 255
```

Exemplo:

```
192.168.0.42
```

### IP estático vs dinâmico

* **Estático:** configurado manualmente
* **Dinâmico:** atribuído automaticamente (DHCP)

---

## 5️⃣ Máscara de rede e CIDR

A máscara define:

* Qual parte do IP identifica a **rede**
* Qual parte identifica o **host**

Exemplo:

```
IP:      192.168.1.10
Máscara: 255.255.255.0
CIDR:    /24
```

Isso significa:

* Rede: 192.168.1.0
* Hosts válidos: 254

---

## 6️⃣ Gateway padrão

O **gateway** é o dispositivo que conecta sua rede local a **outras redes**.

Normalmente é o roteador.

Sem gateway:

* A comunicação local funciona
* A comunicação externa falha

---

## 7️⃣ Portas e serviços

Portas permitem que **vários serviços** usem a rede ao mesmo tempo.

Intervalo total:

```
0 – 65535
```

Faixas:

* 0–1023 → Serviços conhecidos
* 1024–49151 → Registradas
* 49152–65535 → Temporárias

Exemplos:

* 22 → SSH
* 80 → HTTP
* 443 → HTTPS

---

## 8️⃣ Protocolos de transporte

### TCP

* Orientado à conexão
* Confiável
* Ordem garantida

Usado quando **perda de dados não é aceitável**.

### UDP

* Sem conexão
* Não confiável
* Muito rápido

Usado quando **velocidade é mais importante que precisão**.

---

## 9️⃣ DNS — Domain Name System

DNS traduz nomes legíveis em endereços IP.

Exemplo:

```
google.com → 142.xxx.xxx.xxx
```

Tipos comuns de registros:

* A → IPv4
* AAAA → IPv6
* CNAME → Alias

---

## 🔟 Fluxo completo de comunicação

Quando um site é acessado:

1. O domínio é resolvido via DNS
2. O IP é obtido
3. A conexão é criada (TCP)
4. Dados são enviados
5. Resposta é recebida

Esse fluxo é repetido **bilhões de vezes por dia**.

---

## 1️⃣1️⃣ Erros comuns e diagnóstico inicial

### Erro: sem acesso à internet

* IP inexistente → problema local
* Gateway ausente → problema de roteamento
* DNS falhando → nomes não resolvem

Ferramentas iniciais:

```bash
ip a
ip route
ping 8.8.8.8
ping google.com
```

---

## ✅ Resultado esperado ao final dos Fundamentos

Ao concluir esta fase, você será capaz de:

* Entender qualquer diagrama de rede básico
* Saber exatamente **onde** uma conexão pode falhar
* Ler documentação técnica sem se perder
* Avançar para LAN, análise de tráfego e segurança

---

<p align="center">
  <i>"Understanding is the first layer of security."</i>
</p>

---

🧑‍💻 **Mantido por:** Samwns
📡 *Let's all love Lain.*
