---
title: "Установка"
date: 2018-02-23T10:39:42+03:00
weight: 1
---

_React UI Generator_ представляет собою семейство библиотек, построенных вокруг одной центральной библиотеке-ядра: `@react-ui-generator/core`.
Соответственно, процесс установки заключается в подключании этой библиотеки, а также набора вспомогательных бибилотек, в зависимости от нужд разработчика.

## Установка с помощью менеджера пакетов

```shell
npm install @react-ui-generator/core          ## библиотека-ядро
npm install @react-ui-generator/validators    ## библиотека для совместимости с различными валидаторами (Ajv, etc)
npm install @react-ui-generator/serializers   ## библиотека для сериализации сгенерированных форм в JSON, XML, EDN, etc
...
```

Помимо этих пакетов общего назначения, Вам наверняка понадобится один из UI-пакетов, содержащих отрисовщики полей и варианты разметки формы.
Официально, _React UI Generator_ поддерживает следующие UI-наборы:

**Twitter Bootstrap**

```shell
npm install @react-ui-generator/ui-bootstrap
```

**Ant Design**

```shell
npm install @react-ui-generator/ui-antd
```

Однако, благодаря своей модульной архитектуре, _React UI Generator_ позволяет любому разработчику написать свой собственный UI-набор, используемый для генерации форм.
Как правило, это реализуется  в виде тонкой обертки вокруг той или иной UI-библиотеки.