# Instalācijas Instrukcija: MySQL Datubāzes Serveris

## Sistēmas Prasības

- **Operētājsistēma**: Windows, macOS, Linux
- **Procesors**: 1 GHz vai ātrāks
- **Operatīvā atmiņa (RAM)**: Vismaz 512 MB
- **Cietā diska vieta**: Vismaz 1 GB brīvas vietas
- **Interneta savienojums**: Nepieciešams instalācijas failu lejupielādei

## Instalācijas Soļi ar Skaidrojumiem

### 1. Lejupielādēt MySQL Instalācijas Failu

- Apmeklējiet oficiālo MySQL lejupielādes lapu: [MySQL Downloads](https://www.oracle.com/mysql/technologies/mysql-enterprise-edition-downloads.html).

### 2. Izvēlēties Atbilstošo Versiju

- Izvēlieties "MySQL Community Server" un noklikšķiniet uz "Download".

### 3. Lejupielādēt Instalācijas Pakotni

- Izvēlieties instalācijas pakotni, kas atbilst jūsu operētājsistēmai (piemēram, MSI instalētājs Windows sistēmām).

### 4. Palaist Instalētāju

- Atveriet lejupielādēto failu, lai sāktu instalāciju.

### 5. Izvēlēties Instalācijas Veidu

- Instalācijas laikā izvēlieties "Developer Default" vai "Custom", ja vēlaties pielāgot instalāciju.

### 6. Konfigurēt MySQL Serveri

- Iestatiet servera konfigurāciju, piemēram, portu (noklusējuma ir 3306) un autentifikācijas metodi.


### 7. Iestatīt "root" Lietotāja Paroli

- Izvēlieties drošu paroli administratora kontam.

### 8. Pabeigt Instalāciju

- Pārskatiet iestatījumus un noklikšķiniet uz "Execute", lai pabeigtu instalāciju.

## Testēšanas un Konfigurācijas Pamācība

### 1. Pārbaudīt MySQL Servera Darbību

- Atveriet komandrindu un ievadiet `mysql -u root -p`, tad ievadiet savu "root" paroli.

### 2. Izveidot Jaunu Datubāzi

- MySQL konsolē ievadiet `CREATE DATABASE testdb;`.

### 3. Izveidot Jaunu Tabulu un Ievietot Datus

  ```sql
  USE testdb;
  CREATE TABLE users (id INT AUTO_INCREMENT PRIMARY KEY, name VARCHAR(255));
  INSERT INTO users (name) VALUES ('Anna'), ('Jānis');
  ```
 
### 4. Pārbaudīt Ievadītos Datus

- Izpildiet ```SELECT * FROM users;```
