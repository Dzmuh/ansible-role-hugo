# Ansible Role: Hugo

Роль устанавливает (по умолчанию) расширенную версию hugo на системы Ubuntu.

## Зависимости

Нет.

## Параметры роли

Доступные для роли параметры заданы в файле `defaults/main.yml`.

Список доступных параметров:

```yaml
hugo_app: hugo_extended
hugo_version: 0.73.0
hugo_osarch: {{ ansible_system }}-64bit
hugo_dl_url: https://github.com/gohugoio/hugo/releases/download/v{{ hugo_version }}/{{ hugo_app }}_{{ hugo_version }}_{{ hugo_osarch }}.tar.gz
hugo_bin_path: /usr/local/bin
```

## TODO

- [ ] Установка Hugo для текущего пользователя
