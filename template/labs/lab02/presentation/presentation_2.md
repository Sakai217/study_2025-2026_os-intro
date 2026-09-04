---
title: "Лабораторная работа №2"
subtitle: "Базовая настройка git"
author: "Гаджимурадов Аяз Тахирович"
institute: "Группа НБИбд-02-25"
date: "02 сентября 2026 г."
lang: ru-RU
pdf-engine: xelatex
documentclass: beamer
theme: Madrid
colortheme: beaver
fontsize: 11pt
mainfont: "Liberation Serif"
sansfont: "Liberation Sans"
monofont: "Liberation Mono"
---

## Цель работы

Изучить идеологию и применение средств контроля версий.
Освоить умения по работе с git.

## Задание

1. Создать базовую конфигурацию для работы с git.
2. Создать ключ SSH.
3. Создать ключ PGP.
4. Настроить подписи git.
5. Зарегистрироваться на Github.
6. Создать локальный каталог для выполнения заданий по предмету.

## Установка программного обеспечения

Установка git

    Установим git:

    dnf install git

Установка gh
    Fedora:
    dnf install gh
![](image/1.png){width=70%}
 
## Создайте ключи ssh

    по алгоритму rsa с ключём размером 4096 бит:
    ssh-keygen -t rsa -b 4096
    по алгоритму ed25519:
    ssh-keygen -t ed25519
![](image/2.png){width=70%}
    
## Создайте ключи pgp

    Генерируем ключ
    gpg --full-generate-key

![](image/3.png){width=70%}
   
## Добавление PGP ключа в GitHub

Выводим список ключей и копируем отпечаток приватного ключа:
gpg --list-secret-keys --keyid-format LONG
![](image/5.png){width=70%}
Отпечаток ключа — это последовательность байтов, используемая для идентификации более длинного, по сравнению с самим отпечатком ключа.

## Добавление PGP ключа в GitHub

Формат строки:
sec   Алгоритм/Отпечаток_ключа Дата_создания [Флаги] [Годен_до]
      ID_ключа
Cкопируйте ваш сгенерированный PGP ключ в буфер обмена:
gpg --armor --export <PGP Fingerprint> | xclip -sel clip

![](image/6.png){width=70%}
 
## Добавление PGP ключа в GitHub

Перейдите в настройки GitHub (https://github.com/settings/keys), нажмите на кнопку New GPG key и вставьте полученный ключ в поле ввода.

![](image/7.png){width=70%}
 
## 

Спасибо за внимание!

