# Інструкція використання скрипта **kubeplugin**

## Інсталяція

1.1 Скачайте скрипт **kubeplugin** на свій компьютер за допомогою команд:

```bash
 cd ~
 curl -O https://raw.githubusercontent.com/NickP007/les05/main/scripts/kubeplugin
```

1.2 Додайте дозвіл на виконання файлу:

```bash
 chmod +x kubeplugin
```

1.3 Встановіть плагін за допомогою:

```bash
 sudo cp kubeplugin /usr/local/bin/kubectl-kubeplugin
```

1.4 Перевірте наявність встановленого плагіну:

```bash
 kubectl plugin list
```

## Використання

2.1 Запуск **kubeplugin** в якості скрипта:

```bash
 ~/kubeplugin [<resource_type>] [<namespace>]
```

2.2 Запуск **kubeplugin** в якості плагіну **kubectl**:

```bash
 kubectl kubeplugin [<resource_type>] [<namespace>]
```

2.3 Для отримання допомоги введіть:

`~/kubeplugin --help` або  `kubectl kubeplugin --help`

## Приклад

3.1 Приклад використання скрипта **kubeplugin**:

```bash
 ~/kubeplugin default pod
```

> Resource, Namespace, Name, CPU, Memory
>
> pod, default, hello-5db85495d7-8frf9, 17m, 1Mi
>
> pod, default, hello-5db85495d7-g7kgw, 13m, 1Mi
>
> pod, default, hello-5db85495d7-sgp9q, 0m, 1Mi


# Instructions for using the **kubeplugin** script

## Installation

1.1 Download the **kubeplugin** script to your computer using the commands:

```bash
  cd ~
  curl -O https://raw.githubusercontent.com/NickP007/les05/main/scripts/kubeplugin
```

1.2 Add execute permission to the file:

```bash
  chmod +x kubeplugin
```

1.3 Install the plugin using:

```bash
  sudo cp kubeplugin /usr/local/bin/kubectl-kubeplugin
```

1.4 Check for installed plugin:

```bash
  kubectl plugin list
```

## Usage

2.1 Running **kubeplugin** as a script:

```bash
  ~/kubeplugin [<resource_type>] [<namespace>]
```

2.2 Running **kubeplugin** as a **kubectl** plugin:

```bash
  kubectl kubeplugin [<resource_type>] [<namespace>]
```

2.3 To get help, enter:

`~/kubeplugin --help` or `kubectl kubeplugin --help`

## Example

3.1 Example of using the **kubeplugin** script:

```bash
  ~/kubeplugin default pod
```

> Resource, Namespace, Name, CPU, Memory
>
> pod, default, hello-5db85495d7-8frf9, 17m, 1Mi
>
> pod, default, hello-5db85495d7-g7kgw, 13m, 1Mi
>
> pod, default, hello-5db85495d7-sgp9q, 0m, 1Mi
