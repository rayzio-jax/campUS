[![Python](https://img.shields.io/badge/python-v3.11-black?style=for-the-badge&logo=python&labelColor=rgba(202%2C%20173%2C%200%2C%201)&link=https%3A%2F%2Fwww.python.org%2F)](https://www.python.org/)
[![Flask](https://img.shields.io/badge/flask-v2.3.x-black?style=for-the-badge&logo=flask&labelColor=rgba(202%2C%20173%2C%200%2C%201)&link=https%3A%2F%2Fwww.python.org%2F)](https://flask.palletsprojects.com/en/2.3.x/)
[![TailwindCSS](https://img.shields.io/badge/tailwindcss-v3.3.3-black?style=for-the-badge&logo=tailwindcss&labelColor=rgba(0%2C%20156%2C%20249%2C%201)&link=https%3A%2F%2Fwww.python.org%2F)](https://tailwindcss.com/)
[![DaisyUI](https://img.shields.io/badge/daisyui-v3.5.1-black?style=for-the-badge&logo=daisyui&labelColor=rgba(0%2C%20194%2C%2024%2C%201)&link=https%3A%2F%2Fwww.python.org%2F)](https://daisyui.com/)



# campUS
Hey there, lovely peeps! So, imagine this super cool app, like, totally made for all you awesome students out there! 😄 It's, like, a special secret place where you can share your thoughts, questions, or anything with your super cool professors or, like, the big boss, the rector! And guess what? All your messages get this super-duper secret code, so, like, only the magical beings with the right key can read 'em! 🔐✨

And, like, your precious messages? They're all snuggled up, safe and sound, in this super fancy database called PostgreSQL. Ain't that cool? 📚🔒

Oh, and here comes the magical part! Professors and the rector, they got the VIP pass to see all the messages, like, from everyone. But you, sweet student, you only see your own messages, just yours! 😇💌

So, like, why's this here? Well, it's, like, this amazing project for the super smart Computer Security class! It's all about making sure your stuff stays safe and protected while you talk to your profs and the big boss. 🌟💻

In a nutshell, this app is like a cozy corner where students and, like, the super cool academic folks can chat all safe and sound. With messages all coded up and a special safe home for 'em, this app is like a big warm hug for keeping secrets safe. 🤗💌✨


## Our Lecture 💪
<p align="center" valign="top" width="30%">
  <a href="https://hepidad.github.io"><img src="https://media.licdn.com/dms/image/C5603AQE4A3WARH9imA/profile-displayphoto-shrink_800_800/0/1625544749335?e=2147483647&v=beta&t=959ypUT1L34lPjovI6cTMzWiRU3ljb3FfKHzYNX26rQ" width="30%" alt="Irwan Kautsar"/></a><br />
    <b>Irwan Alnarus Kautsar</b><br />
    <b><i>Lecture</i></b>
</p>

## Our Team 🤝

<table>
  <tbody>
  </tbody>
    <tr>
      <td align="center" valign="top" width="30%">
        <a href="https://yuuki0.net"><img src="https://avatars.githubusercontent.com/u/79379934?v=4?s=100" width="100%" alt="ゆうきお ふゆ"/></a><br />
        <b>ゆうきお ふゆ</b><br />
        <b><i>Back-End & Database</i></b>
      </td>
      <td align="center" valign="top" width="30%">
        <a href="https://github.com/AlvitoDian">
          <img src="https://avatars.githubusercontent.com/u/132731944?v=4?s=100" width="100%" alt="Alvito Dian Pratama Putra"/>
        </a><br />
        <b>Alvito Dian Pratama Putra</b><br />
        <b><i>Back-End & Bug Hunter</i></b>
      </td>
      <td align="center" valign="top" width="30%">
        <a href="https://github.com/rayzio-jax">
          <img src="https://avatars.githubusercontent.com/u/111292920?v=4?s=100" width="100%" alt="Rayhanantha Akbar Putra Prasetyo"/>
        </a><br />
        <b>Rayhanantha Akbar</b><br />
        <b><i>Front-End & UI/UX</i></b>
      </td>
    </tr>
  </tbody>
</table>

<hr>

## Screenshots 💻

![image](https://github.com/YuukioFuyu/campUS/assets/79379934/06decb16-9d05-4eed-ad16-9be968e40a5d)
![image](https://github.com/YuukioFuyu/campUS/assets/79379934/6241d387-1949-4acb-a954-36be777bb717)

<hr>

## Dependency

-   Python3
-   PostgreSQL

## Pre-Installation

1. Clone this repository

```bash
git clone https://github.com/YuukioFuyu/campUS.git
```

2. Install python3 & venv

```bash
sudo dnf install python3 python3-venv
```

3. Install postgreSQL database

```bash
sudo dnf install postgresql14-server
```

4. Setup postgreSQL

```bash
sudo /usr/pgsql-14/bin/postgresql-14-setup initdb
```

5. Enable postgreSQL services

```bash
sudo systemctl enable --now postgresql-14
```

6. Create database

```bash
psql -U postgres
```
```bash
create database messages;
```
```bash
\q
```

7. Import database

```bash
psql -U postgres messages < messages.psql
```

## Installation

1. Create venv directory

```bash
python3 -m venv [path to venv]
```

2. Enable venv

```bash
source [path to venv]/bin/activate
```

3. Install requirements

```bash
pip install -r requirements.txt
```

4. Edit app.py

### Customise with your settings
- app.config['SQLALCHEMY_DATABASE_URI'] = 'postgresql://[DATABASE USER]:[PASSWORD]@[IP SERVER]/[DATABASE NAME]'
- app.secret_key = 'YOUR SECRET KEY'

5. Save and exit app.py

6. Run the program

```bash
python3 ./app.py
```

7. Access via browser on localhost / http://127.0.0.1

<hr>

### Default Login:
#### Administrator
| Username | Password |
|  ------- | -------- |
|   admin  |   admin  |

#### Student 1
| Username | Password |
|  ------- | -------- |
|    mhs1  |    mhs1  |

#### Student 2
| Username | Password |
|  ------- | -------- |
|    mhs2  |    mhs2  |
