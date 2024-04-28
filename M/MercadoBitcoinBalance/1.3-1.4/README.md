# Comparing `tmp/mercadobitcoinbalance-1.3.tar.gz` & `tmp/mercadobitcoinbalance-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mercadobitcoinbalance-1.3.tar", last modified: Fri Apr 12 21:37:05 2024, max compression
+gzip compressed data, was "mercadobitcoinbalance-1.4.tar", last modified: Sun Apr 28 16:49:05 2024, max compression
```

## Comparing `mercadobitcoinbalance-1.3.tar` & `mercadobitcoinbalance-1.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 aviram    (1000) aviram    (1000)        0 2024-04-12 21:37:05.000000 mercadobitcoinbalance-1.3/
--rw-r--r--   0 aviram    (1000) aviram    (1000)    35149 2023-11-28 19:52:03.000000 mercadobitcoinbalance-1.3/LICENSE
-drwxr-xr-x   0 aviram    (1000) aviram    (1000)        0 2024-04-12 21:37:04.000000 mercadobitcoinbalance-1.3/MercadoBitcoinBalance.egg-info/
--rw-r--r--   0 aviram    (1000) aviram    (1000)    44909 2024-04-12 21:37:02.000000 mercadobitcoinbalance-1.3/MercadoBitcoinBalance.egg-info/PKG-INFO
--rw-r--r--   0 aviram    (1000) aviram    (1000)      336 2024-04-12 21:37:02.000000 mercadobitcoinbalance-1.3/MercadoBitcoinBalance.egg-info/SOURCES.txt
--rw-r--r--   0 aviram    (1000) aviram    (1000)        1 2024-04-12 21:37:02.000000 mercadobitcoinbalance-1.3/MercadoBitcoinBalance.egg-info/dependency_links.txt
--rw-r--r--   0 aviram    (1000) aviram    (1000)       66 2024-04-12 21:37:02.000000 mercadobitcoinbalance-1.3/MercadoBitcoinBalance.egg-info/entry_points.txt
--rw-r--r--   0 aviram    (1000) aviram    (1000)        7 2024-04-12 21:37:02.000000 mercadobitcoinbalance-1.3/MercadoBitcoinBalance.egg-info/requires.txt
--rw-r--r--   0 aviram    (1000) aviram    (1000)       22 2024-04-12 21:37:02.000000 mercadobitcoinbalance-1.3/MercadoBitcoinBalance.egg-info/top_level.txt
--rw-r--r--   0 aviram    (1000) aviram    (1000)    44909 2024-04-12 21:37:05.000000 mercadobitcoinbalance-1.3/PKG-INFO
--rw-r--r--   0 aviram    (1000) aviram    (1000)     3385 2023-12-17 05:45:36.000000 mercadobitcoinbalance-1.3/README.md
--rw-r--r--   0 aviram    (1000) aviram    (1000)     1126 2024-04-12 21:35:38.000000 mercadobitcoinbalance-1.3/pyproject.toml
--rw-r--r--   0 aviram    (1000) aviram    (1000)       38 2024-04-12 21:37:05.000000 mercadobitcoinbalance-1.3/setup.cfg
-drwxr-xr-x   0 aviram    (1000) aviram    (1000)        0 2024-04-12 21:37:04.000000 mercadobitcoinbalance-1.3/src/
--rw-r--r--   0 aviram    (1000) aviram    (1000)     4597 2023-11-28 19:52:03.000000 mercadobitcoinbalance-1.3/src/__init__.py
--rw-r--r--   0 aviram    (1000) aviram    (1000)    11482 2024-04-12 21:35:02.000000 mercadobitcoinbalance-1.3/src/__main__.py
+drwxr-xr-x   0 aviram    (1000) aviram    (1000)        0 2024-04-28 16:49:05.000000 mercadobitcoinbalance-1.4/
+-rw-r--r--   0 aviram    (1000) aviram    (1000)    35149 2023-11-28 19:52:03.000000 mercadobitcoinbalance-1.4/LICENSE
+drwxr-xr-x   0 aviram    (1000) aviram    (1000)        0 2024-04-28 16:49:05.000000 mercadobitcoinbalance-1.4/MercadoBitcoinBalance.egg-info/
+-rw-r--r--   0 aviram    (1000) aviram    (1000)    45433 2024-04-28 16:49:05.000000 mercadobitcoinbalance-1.4/MercadoBitcoinBalance.egg-info/PKG-INFO
+-rw-r--r--   0 aviram    (1000) aviram    (1000)      336 2024-04-28 16:49:05.000000 mercadobitcoinbalance-1.4/MercadoBitcoinBalance.egg-info/SOURCES.txt
+-rw-r--r--   0 aviram    (1000) aviram    (1000)        1 2024-04-28 16:49:05.000000 mercadobitcoinbalance-1.4/MercadoBitcoinBalance.egg-info/dependency_links.txt
+-rw-r--r--   0 aviram    (1000) aviram    (1000)       66 2024-04-28 16:49:05.000000 mercadobitcoinbalance-1.4/MercadoBitcoinBalance.egg-info/entry_points.txt
+-rw-r--r--   0 aviram    (1000) aviram    (1000)        7 2024-04-28 16:49:05.000000 mercadobitcoinbalance-1.4/MercadoBitcoinBalance.egg-info/requires.txt
+-rw-r--r--   0 aviram    (1000) aviram    (1000)       22 2024-04-28 16:49:05.000000 mercadobitcoinbalance-1.4/MercadoBitcoinBalance.egg-info/top_level.txt
+-rw-r--r--   0 aviram    (1000) aviram    (1000)    45433 2024-04-28 16:49:05.000000 mercadobitcoinbalance-1.4/PKG-INFO
+-rw-r--r--   0 aviram    (1000) aviram    (1000)     3909 2024-04-28 16:47:27.000000 mercadobitcoinbalance-1.4/README.md
+-rw-r--r--   0 aviram    (1000) aviram    (1000)     1126 2024-04-28 14:23:46.000000 mercadobitcoinbalance-1.4/pyproject.toml
+-rw-r--r--   0 aviram    (1000) aviram    (1000)       38 2024-04-28 16:49:05.000000 mercadobitcoinbalance-1.4/setup.cfg
+drwxr-xr-x   0 aviram    (1000) aviram    (1000)        0 2024-04-28 16:49:05.000000 mercadobitcoinbalance-1.4/src/
+-rw-r--r--   0 aviram    (1000) aviram    (1000)     5376 2024-04-28 14:32:44.000000 mercadobitcoinbalance-1.4/src/__init__.py
+-rw-r--r--   0 aviram    (1000) aviram    (1000)    12175 2024-04-28 16:37:09.000000 mercadobitcoinbalance-1.4/src/__main__.py
```

### Comparing `mercadobitcoinbalance-1.3/LICENSE` & `mercadobitcoinbalance-1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mercadobitcoinbalance-1.3/MercadoBitcoinBalance.egg-info/PKG-INFO` & `mercadobitcoinbalance-1.4/MercadoBitcoinBalance.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MercadoBitcoinBalance
-Version: 1.3
+Version: 1.4
 Summary: Calcula, salva e reporta seu saldo do Mercado Bitcoin
 Author-email: Avi Alkalay <avi@unix.sh>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -699,15 +699,35 @@
 Este programa:
 
 - Busca saldo em BRL de todos os seus tokens no Mercado Bitcoin
 - Calcula saldo consolidado
 - Atualiza um CSV caso o saldo tenha mudado
 - Manda o saldo atual por e-mail ou Telegram junto com algumas estatísticas
 
-## Como usá-lo
+É necessário Python 3, Pandas e nada mais para rodar este programa.
+
+Para conseguir enviar e-mails, seu sistema (Linux, obviamente) de forma geral precisa estar configurado como cliente de mail. [Eis um exemplo para configurar o postfix do Fedora](https://fedoramagazine.org/use-postfix-to-get-email-from-your-fedora-system/).
+
+Depois, eu uso o CSV junto com o [investorzilla](https://github.com/avibrazil/investorzilla) para acompanhar performance.
+
+# Como usar a API
+
+```python
+import MercadoBitcoinBalance
+
+# Suas credenciais obtidas em https://www.MercadoBitcoin.com.br/plataforma/chaves-api
+MP_API_ID='06…05'
+MP_API_SECRET='10…19'
+
+mb=MercadoBitcoinBalance.MercadoBitcoinAPI(MP_API_ID,MP_API_SECRET)
+
+balances=mb.get_BRL_balances()
+```
+
+# Como usar na linha de comando
 
 Instale:
 
 ```shell
 pip install MercadoBitcoinBalance --user
 ```
 
@@ -728,25 +748,25 @@
 
 Sendo:
 
 - `mb-id` e `mb-secret`: suas credenciais obtidas em https://www.MercadoBitcoin.com.br/plataforma/chaves-api
 - `csv-threshold`: só atualiza CSV se variação do saldo é maior do que este valor
 - `csv`: nome do arquivo CSV para registrar o saldo
 - `csv-fund-name`: um nome qualquer para etiquetar o saldo no CSV
-- `report-threshold`: só manda relatório se variação do saldo é maior do que este valor
+- `report-threshold`: só manda relatório se variação do saldo, desde último relatório, é maior do que este valor
 - `mail`: endereço para enviar pequeno relatório por e-mail; não manda se omitido
 - `telegram-chat-id`: o ID do seu usuário Telegram; não manda se omitido
 - `telegram-bot-id`: o ID do bot que você deve criar em https://t.me/BotFather
 
 O CSV acumula os valores como uma série temoral. Registra a hora UTC (UTC, sempre UTC, sempre), o nome do fundo (passado em `csv-fund-name`) e o saldo consolidado em BRL. Assim:
 
 ```csv
-time|fund|BRL
-2023-05-31T19:30:47.407006+00:00|Nome arbitrário do fundo|36595.57
-2023-05-31T20:50:14.708121+00:00|Nome arbitrário do fundo|36576.22
+time|fund|BRL|reported
+2023-05-31T19:30:47.407006+00:00|Nome arbitrário do fundo|36595.57|1
+2023-05-31T20:50:14.708121+00:00|Nome arbitrário do fundo|36576.22|0
 ```
 
 O e-mail e mensagem de Telegram enviados tem esta cara:
 
 > Current balance: **36,576.22 BRL**.
 >
 > Previous balance: **34,595.72 BRL**.
@@ -765,19 +785,17 @@
 > | **abfy** | 336\.42 BRL |
 > | **psgft** | 9\.40 BRL |
 > | **wemix** | 0\.54 BRL |
 
 Eu rodo isso a cada meia hora via crontab, assim:
 
 ```crontab
-*/30 * * * * ~/.local/bin/balancemb --mb-id 06…05 --mb-secret 10…19 --csv-threshold 2 --csv ~/investorzilla/mercadobitcoin-balances.txt --csv-fund-name 'Nome arbitrário do fundo' --report-threshold 20 --telegram-chat-id 12345678 --telegram-bot-id '11223344::A…k'
-15 20 * * * ~/.local/bin/balancemb --mb-id 06…05 --mb-secret 10…19 --csv-threshold 5 --csv ~/investorzilla/mercadobitcoin-balances.txt --csv-fund-name 'Nome arbitrário do fundo' --report-threshold -1 --telegram-chat-id 12345678 --telegram-bot-id '11223344::A…k'
+*/30 * * * * ~/.local/bin/balancemb --mb-id 06…05 --mb-secret 10…19 --csv-threshold 2 --csv ~/investorzilla-my/mercadobitcoin-balances.txt --csv-fund-name 'Nome arbitrário do fundo' --report-threshold 20 --telegram-chat-id 12345678 --telegram-bot-id '11223344::A…k'
 ```
 
-Ou seja, atualizo saldo consolidado em `balances.txt` a cada meia hora, não mando e-mail mas mando saldos por Telegram caso houver variação de mais de 20 BRL.
-Além do mais, todo dia às 20:15 manda o saldo atual.
-
-É necessário Python 3, Pandas e nada mais para rodar este programa.
-
-Para conseguir enviar e-mails, seu sistema (Linux, obviamente) de forma geral precisa estar configurado como cliente de mail. [Eis um exemplo para configurar o postfix do Fedora](https://fedoramagazine.org/use-postfix-to-get-email-from-your-fedora-system/).
+Adicionalmente, rodo todos os dias às 20:15 e forço envio de relatório (`--report-threshold -1`) por Telegram:
+```crontab
+15 20 * * * ~/.local/bin/balancemb --mb-id 06…05 --mb-secret 10…19 --csv-threshold 5 --csv ~/investorzilla-my/mercadobitcoin-balances.txt --csv-fund-name 'Nome arbitrário do fundo' --report-threshold -1 --telegram-chat-id 12345678 --telegram-bot-id '11223344::A…k'
+```
 
-Depois, eu uso o CSV junto com o [investorzilla](https://github.com/avibrazil/investorzilla) para acompanhar performance.
+Ou seja, atualizo saldo consolidado em `balances.txt` a cada meia hora, não mando relatório mas mando saldos por Telegram caso houver variação de mais de 20 BRL.
+Além do mais, todo dia às 20:15 manda o saldo atual, mesmo que não houve variação.
```

### Comparing `mercadobitcoinbalance-1.3/PKG-INFO` & `mercadobitcoinbalance-1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MercadoBitcoinBalance
-Version: 1.3
+Version: 1.4
 Summary: Calcula, salva e reporta seu saldo do Mercado Bitcoin
 Author-email: Avi Alkalay <avi@unix.sh>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -699,15 +699,35 @@
 Este programa:
 
 - Busca saldo em BRL de todos os seus tokens no Mercado Bitcoin
 - Calcula saldo consolidado
 - Atualiza um CSV caso o saldo tenha mudado
 - Manda o saldo atual por e-mail ou Telegram junto com algumas estatísticas
 
-## Como usá-lo
+É necessário Python 3, Pandas e nada mais para rodar este programa.
+
+Para conseguir enviar e-mails, seu sistema (Linux, obviamente) de forma geral precisa estar configurado como cliente de mail. [Eis um exemplo para configurar o postfix do Fedora](https://fedoramagazine.org/use-postfix-to-get-email-from-your-fedora-system/).
+
+Depois, eu uso o CSV junto com o [investorzilla](https://github.com/avibrazil/investorzilla) para acompanhar performance.
+
+# Como usar a API
+
+```python
+import MercadoBitcoinBalance
+
+# Suas credenciais obtidas em https://www.MercadoBitcoin.com.br/plataforma/chaves-api
+MP_API_ID='06…05'
+MP_API_SECRET='10…19'
+
+mb=MercadoBitcoinBalance.MercadoBitcoinAPI(MP_API_ID,MP_API_SECRET)
+
+balances=mb.get_BRL_balances()
+```
+
+# Como usar na linha de comando
 
 Instale:
 
 ```shell
 pip install MercadoBitcoinBalance --user
 ```
 
@@ -728,25 +748,25 @@
 
 Sendo:
 
 - `mb-id` e `mb-secret`: suas credenciais obtidas em https://www.MercadoBitcoin.com.br/plataforma/chaves-api
 - `csv-threshold`: só atualiza CSV se variação do saldo é maior do que este valor
 - `csv`: nome do arquivo CSV para registrar o saldo
 - `csv-fund-name`: um nome qualquer para etiquetar o saldo no CSV
-- `report-threshold`: só manda relatório se variação do saldo é maior do que este valor
+- `report-threshold`: só manda relatório se variação do saldo, desde último relatório, é maior do que este valor
 - `mail`: endereço para enviar pequeno relatório por e-mail; não manda se omitido
 - `telegram-chat-id`: o ID do seu usuário Telegram; não manda se omitido
 - `telegram-bot-id`: o ID do bot que você deve criar em https://t.me/BotFather
 
 O CSV acumula os valores como uma série temoral. Registra a hora UTC (UTC, sempre UTC, sempre), o nome do fundo (passado em `csv-fund-name`) e o saldo consolidado em BRL. Assim:
 
 ```csv
-time|fund|BRL
-2023-05-31T19:30:47.407006+00:00|Nome arbitrário do fundo|36595.57
-2023-05-31T20:50:14.708121+00:00|Nome arbitrário do fundo|36576.22
+time|fund|BRL|reported
+2023-05-31T19:30:47.407006+00:00|Nome arbitrário do fundo|36595.57|1
+2023-05-31T20:50:14.708121+00:00|Nome arbitrário do fundo|36576.22|0
 ```
 
 O e-mail e mensagem de Telegram enviados tem esta cara:
 
 > Current balance: **36,576.22 BRL**.
 >
 > Previous balance: **34,595.72 BRL**.
@@ -765,19 +785,17 @@
 > | **abfy** | 336\.42 BRL |
 > | **psgft** | 9\.40 BRL |
 > | **wemix** | 0\.54 BRL |
 
 Eu rodo isso a cada meia hora via crontab, assim:
 
 ```crontab
-*/30 * * * * ~/.local/bin/balancemb --mb-id 06…05 --mb-secret 10…19 --csv-threshold 2 --csv ~/investorzilla/mercadobitcoin-balances.txt --csv-fund-name 'Nome arbitrário do fundo' --report-threshold 20 --telegram-chat-id 12345678 --telegram-bot-id '11223344::A…k'
-15 20 * * * ~/.local/bin/balancemb --mb-id 06…05 --mb-secret 10…19 --csv-threshold 5 --csv ~/investorzilla/mercadobitcoin-balances.txt --csv-fund-name 'Nome arbitrário do fundo' --report-threshold -1 --telegram-chat-id 12345678 --telegram-bot-id '11223344::A…k'
+*/30 * * * * ~/.local/bin/balancemb --mb-id 06…05 --mb-secret 10…19 --csv-threshold 2 --csv ~/investorzilla-my/mercadobitcoin-balances.txt --csv-fund-name 'Nome arbitrário do fundo' --report-threshold 20 --telegram-chat-id 12345678 --telegram-bot-id '11223344::A…k'
 ```
 
-Ou seja, atualizo saldo consolidado em `balances.txt` a cada meia hora, não mando e-mail mas mando saldos por Telegram caso houver variação de mais de 20 BRL.
-Além do mais, todo dia às 20:15 manda o saldo atual.
-
-É necessário Python 3, Pandas e nada mais para rodar este programa.
-
-Para conseguir enviar e-mails, seu sistema (Linux, obviamente) de forma geral precisa estar configurado como cliente de mail. [Eis um exemplo para configurar o postfix do Fedora](https://fedoramagazine.org/use-postfix-to-get-email-from-your-fedora-system/).
+Adicionalmente, rodo todos os dias às 20:15 e forço envio de relatório (`--report-threshold -1`) por Telegram:
+```crontab
+15 20 * * * ~/.local/bin/balancemb --mb-id 06…05 --mb-secret 10…19 --csv-threshold 5 --csv ~/investorzilla-my/mercadobitcoin-balances.txt --csv-fund-name 'Nome arbitrário do fundo' --report-threshold -1 --telegram-chat-id 12345678 --telegram-bot-id '11223344::A…k'
+```
 
-Depois, eu uso o CSV junto com o [investorzilla](https://github.com/avibrazil/investorzilla) para acompanhar performance.
+Ou seja, atualizo saldo consolidado em `balances.txt` a cada meia hora, não mando relatório mas mando saldos por Telegram caso houver variação de mais de 20 BRL.
+Além do mais, todo dia às 20:15 manda o saldo atual, mesmo que não houve variação.
```

### Comparing `mercadobitcoinbalance-1.3/README.md` & `mercadobitcoinbalance-1.4/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -3,15 +3,35 @@
 Este programa:
 
 - Busca saldo em BRL de todos os seus tokens no Mercado Bitcoin
 - Calcula saldo consolidado
 - Atualiza um CSV caso o saldo tenha mudado
 - Manda o saldo atual por e-mail ou Telegram junto com algumas estatísticas
 
-## Como usá-lo
+É necessário Python 3, Pandas e nada mais para rodar este programa.
+
+Para conseguir enviar e-mails, seu sistema (Linux, obviamente) de forma geral precisa estar configurado como cliente de mail. [Eis um exemplo para configurar o postfix do Fedora](https://fedoramagazine.org/use-postfix-to-get-email-from-your-fedora-system/).
+
+Depois, eu uso o CSV junto com o [investorzilla](https://github.com/avibrazil/investorzilla) para acompanhar performance.
+
+# Como usar a API
+
+```python
+import MercadoBitcoinBalance
+
+# Suas credenciais obtidas em https://www.MercadoBitcoin.com.br/plataforma/chaves-api
+MP_API_ID='06…05'
+MP_API_SECRET='10…19'
+
+mb=MercadoBitcoinBalance.MercadoBitcoinAPI(MP_API_ID,MP_API_SECRET)
+
+balances=mb.get_BRL_balances()
+```
+
+# Como usar na linha de comando
 
 Instale:
 
 ```shell
 pip install MercadoBitcoinBalance --user
 ```
 
@@ -32,25 +52,25 @@
 
 Sendo:
 
 - `mb-id` e `mb-secret`: suas credenciais obtidas em https://www.MercadoBitcoin.com.br/plataforma/chaves-api
 - `csv-threshold`: só atualiza CSV se variação do saldo é maior do que este valor
 - `csv`: nome do arquivo CSV para registrar o saldo
 - `csv-fund-name`: um nome qualquer para etiquetar o saldo no CSV
-- `report-threshold`: só manda relatório se variação do saldo é maior do que este valor
+- `report-threshold`: só manda relatório se variação do saldo, desde último relatório, é maior do que este valor
 - `mail`: endereço para enviar pequeno relatório por e-mail; não manda se omitido
 - `telegram-chat-id`: o ID do seu usuário Telegram; não manda se omitido
 - `telegram-bot-id`: o ID do bot que você deve criar em https://t.me/BotFather
 
 O CSV acumula os valores como uma série temoral. Registra a hora UTC (UTC, sempre UTC, sempre), o nome do fundo (passado em `csv-fund-name`) e o saldo consolidado em BRL. Assim:
 
 ```csv
-time|fund|BRL
-2023-05-31T19:30:47.407006+00:00|Nome arbitrário do fundo|36595.57
-2023-05-31T20:50:14.708121+00:00|Nome arbitrário do fundo|36576.22
+time|fund|BRL|reported
+2023-05-31T19:30:47.407006+00:00|Nome arbitrário do fundo|36595.57|1
+2023-05-31T20:50:14.708121+00:00|Nome arbitrário do fundo|36576.22|0
 ```
 
 O e-mail e mensagem de Telegram enviados tem esta cara:
 
 > Current balance: **36,576.22 BRL**.
 >
 > Previous balance: **34,595.72 BRL**.
@@ -69,19 +89,17 @@
 > | **abfy** | 336\.42 BRL |
 > | **psgft** | 9\.40 BRL |
 > | **wemix** | 0\.54 BRL |
 
 Eu rodo isso a cada meia hora via crontab, assim:
 
 ```crontab
-*/30 * * * * ~/.local/bin/balancemb --mb-id 06…05 --mb-secret 10…19 --csv-threshold 2 --csv ~/investorzilla/mercadobitcoin-balances.txt --csv-fund-name 'Nome arbitrário do fundo' --report-threshold 20 --telegram-chat-id 12345678 --telegram-bot-id '11223344::A…k'
-15 20 * * * ~/.local/bin/balancemb --mb-id 06…05 --mb-secret 10…19 --csv-threshold 5 --csv ~/investorzilla/mercadobitcoin-balances.txt --csv-fund-name 'Nome arbitrário do fundo' --report-threshold -1 --telegram-chat-id 12345678 --telegram-bot-id '11223344::A…k'
+*/30 * * * * ~/.local/bin/balancemb --mb-id 06…05 --mb-secret 10…19 --csv-threshold 2 --csv ~/investorzilla-my/mercadobitcoin-balances.txt --csv-fund-name 'Nome arbitrário do fundo' --report-threshold 20 --telegram-chat-id 12345678 --telegram-bot-id '11223344::A…k'
 ```
 
-Ou seja, atualizo saldo consolidado em `balances.txt` a cada meia hora, não mando e-mail mas mando saldos por Telegram caso houver variação de mais de 20 BRL.
-Além do mais, todo dia às 20:15 manda o saldo atual.
-
-É necessário Python 3, Pandas e nada mais para rodar este programa.
-
-Para conseguir enviar e-mails, seu sistema (Linux, obviamente) de forma geral precisa estar configurado como cliente de mail. [Eis um exemplo para configurar o postfix do Fedora](https://fedoramagazine.org/use-postfix-to-get-email-from-your-fedora-system/).
+Adicionalmente, rodo todos os dias às 20:15 e forço envio de relatório (`--report-threshold -1`) por Telegram:
+```crontab
+15 20 * * * ~/.local/bin/balancemb --mb-id 06…05 --mb-secret 10…19 --csv-threshold 5 --csv ~/investorzilla-my/mercadobitcoin-balances.txt --csv-fund-name 'Nome arbitrário do fundo' --report-threshold -1 --telegram-chat-id 12345678 --telegram-bot-id '11223344::A…k'
+```
 
-Depois, eu uso o CSV junto com o [investorzilla](https://github.com/avibrazil/investorzilla) para acompanhar performance.
+Ou seja, atualizo saldo consolidado em `balances.txt` a cada meia hora, não mando relatório mas mando saldos por Telegram caso houver variação de mais de 20 BRL.
+Além do mais, todo dia às 20:15 manda o saldo atual, mesmo que não houve variação.
```

### Comparing `mercadobitcoinbalance-1.3/pyproject.toml` & `mercadobitcoinbalance-1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 [project]
 name = "MercadoBitcoinBalance"
-version = '1.3'
+version = '1.4'
 description = "Calcula, salva e reporta seu saldo do Mercado Bitcoin"
 readme = "README.md"
 license = { file = "LICENSE" }
 requires-python = ">=3.8"
 authors = [
     { name = "Avi Alkalay", email = "avi@unix.sh" },
 ]
```

### Comparing `mercadobitcoinbalance-1.3/src/__main__.py` & `mercadobitcoinbalance-1.4/src/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 import pandas
 
 import MercadoBitcoinBalance
 
 
 def send_telegram_report(chat_id,bot_id,tokens):
     """
-    Send a report via telegram.
+    Send a report via Telegram API.
     """
 
     url_message="https://api.telegram.org/bot{bot_id}/sendMessage?parse_mode=html&chat_id={chat_id}&text={message}"
     url_graph="https://api.telegram.org/bot{bot_id}/sendPhoto"
 
     template=[
         'Current balance: <strong>{balance:,.2f} BRL</strong>.\n',
@@ -47,32 +47,14 @@
                 bot_id=bot_id,
                 chat_id=chat_id,
                 message=message
             )
         )
     )
 
-    # with io.BytesIO() as buffer:  # use buffer memory
-    #     tokens['balance_history'].plot(kind='line').figure.savefig(buffer, format='png')
-    #     buffer.seek(0)
-
-    #     graph = dict(
-    #         chat_id=chat_id,
-    #         caption='something',
-    #         photo=buffer.read()
-    #     )
-
-    # urllib.request.urlopen(
-    #     urllib.request.Request(
-    #         url=url_graph.format(bot_id=bot_id),
-    #         data=urllib.parse.urlencode(graph).encode()
-    #     )
-    # )
-
-    # print(urllib.parse.urlencode(graph).encode()[:200])
 
 
 def send_mail_report(recipient,tokens):
     """
     Use system mailer to send a well formatted e-mail.
     """
     template_subject='Mercado Bitcoin new balance: {balance:,.2f} BRL'
@@ -101,33 +83,36 @@
     with smtplib.SMTP() as smtp:
         smtp.connect()
         smtp.sendmail('', recipient, msg.as_string())
 
 
 
 def prepare_logging(level=logging.INFO):
-    # Switch between INFO/DEBUG while running in production/developping:
+    # Switch between INFO/DEBUG while running in production/development:
 
-    # Configure logging for Robson
+    # Configure logging
 
-    FORMATTER = logging.Formatter("%(asctime)s|%(levelname)s|%(name)s|%(message)s")
     HANDLER = logging.StreamHandler()
-    HANDLER.setFormatter(FORMATTER)
+    HANDLER.setFormatter(
+        logging.Formatter("%(asctime)s|%(levelname)s|%(name)s|%(message)s")
+    )
 
-    loggers=[
-        logging.getLogger('__main__'),
-        logging.getLogger('urllib'),
-        logging.getLogger('pandas')
+    logger_domains=[
+        'urllib',
+        'pandas',
+        'MercadoBitcoinBalance',
+        '__main__',
     ]
 
-    for logger in loggers:
+    for logger in logger_domains:
+        logger=logging.getLogger(logger)
         logger.addHandler(HANDLER)
         logger.setLevel(level)
 
-    return loggers[0]
+    return logger
 
 
 
 def prepare_args():
     parser = argparse.ArgumentParser(
         prog='balancemb',
         description='Get consolidated balance from Mercado Bitcoin. Optionaly send it by e-mail and write to CSV file.'
@@ -174,15 +159,15 @@
 
     parser.add_argument(
         '--report-threshold',
         dest='report_threshold',
         required=False,
         type=float,
         default=2,
-        help='Send report only if balance variation is bigger than this'
+        help='Send Telegram or mail report only if balance variation is bigger than this'
     )
 
     parser.add_argument(
         '--mail',
         dest='mail_recipient',
         required=False,
         default=None,
@@ -214,14 +199,15 @@
     )
 
     parsed = parser.parse_args()
 
     return parsed.__dict__
 
 
+
 def main():
     # Read environment and command line parameters
     args=prepare_args()
 
     # Setup logging
     global logger
     if args['DEBUG']:
@@ -232,113 +218,148 @@
           opener = urllib.request.build_opener(http_handler, https_handler)
         except ImportError:
           opener = urllib.request.build_opener(http_handler)
         urllib.request.install_opener(opener)
     else:
         logger=prepare_logging()
 
-    mb=MercadoBitcoinBalance.MercadoBitcoinAPI(args['MP_API_ID'],args['MP_API_SECRET'])
+    mb=MercadoBitcoinBalance.MercadoBitcoinAPI(
+        api_id     = args['MP_API_ID'],
+        api_secret = args['MP_API_SECRET']
+    )
 
     balances=mb.get_BRL_balances()
 
+    # Make a one-line DataFrame
     balance=pandas.DataFrame(
         data=dict(
             fund  = args['csv_fund_name'],
             BRL   = balances.sum().values[0]
         ),
-        index=pandas.DatetimeIndex([pandas.Timestamp.now(tz='UTC')], name='time')
+        index=pandas.DatetimeIndex(
+            [pandas.Timestamp.now(tz='UTC')],
+            name='time'
+        )
     )
 
+    logger.debug("Balance:\n" + balance.to_markdown())
+
     balance_change_for_report=True
     balance_change_for_csv=True
     balance_prev=None
     csv=None
 
     if args['csv_file_name']:
         try:
             csv=pandas.read_csv(
                 args['csv_file_name'],
                 parse_dates=[0],
                 index_col=0,
-                sep='|'
+                dtype=dict(reported='Int8'),
+                sep='|',
             ).sort_index()
         except FileNotFoundError:
             csv=None
 
         if csv is not None:
             # CSV exists.
 
             # Determine if we still want to save to CSV or send report
             balance_prev=csv.tail(1).BRL.values[0]
+            try:
+                balance_prev_reported=(
+                    csv
+                    .fillna(0)
+                    .query('reported==1', engine='python')
+                    .tail(1)
+                    .BRL
+                    .values[0]
+                )
+            except IndexError:
+                # Balance was never reported before
+                balance_prev_reported=0
 
-            balance_change_for_csv=(
-                abs(
-                    balance.BRL.sum() -
-                    balance_prev
-                )>args['csv_threshold']
-            )
-
+            # Decide if we'll send a report when current distance to last
+            # balance reported is bigger than report_threshold
             balance_change_for_report=(
                 abs(
                     balance.BRL.sum() -
-                    balance_prev
+                    balance_prev_reported
                 )>args['report_threshold']
             )
 
+            if balance_change_for_report:
+                # Write CSV anyway if we are sending a report
+                balance_change_for_csv = True
+            else:
+                balance_change_for_csv=(
+                    abs(
+                        balance.BRL.sum() -
+                        balance_prev
+                    )>args['csv_threshold']
+                )
+
             # CSV writting parameters
             to_csv_mode='a'
             to_csv_header=False
         else:
+            # CSV doesn't exists.
+
             # Set to send report because this is the first run
             balance_change_for_csv=True
             balance_change_for_report=True
 
-            # CSV doesn't exist.
             # CSV writting parameters
             to_csv_mode='w'
             to_csv_header=True
 
         # Append to an existent CSV only if balance changed
         if balance_change_for_csv:
             (
+                # Write or append the one-line balance
                 balance
                 .reset_index()
-                .assign(time=lambda table: table.time.apply(lambda timecell: timecell.isoformat()))
-            ).to_csv(
-                args['csv_file_name'],
-                sep='|',
-                index=False,
-                header=to_csv_header,
-                mode=to_csv_mode,
+                .assign(
+                    time=lambda table: table.time.apply(lambda timecell: timecell.isoformat()),
+                    reported=int(balance_change_for_report),
+                )
+                .to_csv(
+                    args['csv_file_name'],
+                    sep='|',
+                    index=False,
+                    header=to_csv_header,
+                    mode=to_csv_mode,  # append or complete write
+                )
             )
 
         # Now reload a complete and up to date CSV
         balance_history=pandas.read_csv(
             args['csv_file_name'],
             parse_dates=[0],
             index_col=0,
-            sep='|'
+            dtype=dict(reported='Int8'),
+            sep='|',
         ).sort_index()
 
     else: # no CSV
         balance_history=balance
 
     # At this point we have the following:
     # - balances: DataFrame with BRL balance per token
-    # - balance_history: Time series of summarized balances
+    # - balance_history: Time series of summarized balance
     # - balance_prev: Previous balance (only if historical CSV available)
 
     # Function to merge several dicts
     dmerge = lambda *args: dict(itertools.chain(*[d.items() for d in args]))
 
     report_tokens=dict(
         balance_history  = balance_history,
         balances         = balances,
         balance          = balance_history.tail(1).BRL.values[0],
-        balance_prev     = balance_prev
+        balance_prev     = balance_prev_reported
     )
 
     report_tokens=dmerge(
         report_tokens,
         dict(
             balance_var      = report_tokens['balance']-report_tokens['balance_prev'],
             balance_pct_change = (report_tokens['balance']/report_tokens['balance_prev'])-1,
```

