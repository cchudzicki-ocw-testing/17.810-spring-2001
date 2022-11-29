---
content_type: page
description: testing subscripts and superscripts
draft: false
title: Subscripts and Superscripts
uid: d8b66928-ee87-4b59-ac37-d78f781e73e6
---
**NOTE:** Not all of these are use-cases that we want to encourage. The goal here is to document what currently works and to alert ourselves if one of these stops breaking. For example, styling bold inside a subscript is absolutely not something we would encourage..

Example, Normal: Lorem ipsum dolor sit<sub>abc 123</sub> amet consectetur. Lorem ipsum dolor sit<sup>abc 123</sup> amet consectetur.

Example, Bold: **Lorem ipsum dolor sit<sub>abc 123</sub> amet consectetur. Lorem ipsum dolor sit<sup>abc 123</sup> amet consectetur.**

Example, Italic: *Lorem ipsum dolor sit<sub>abc 123</sub> amet consectetur. Lorem ipsum dolor sit<sup>abc 123</sup> amet consectetur.*

Example, Interior Bold: Lorem ipsum dolor sit<sub>abc </sub> **<sub>123</sub>** amet consectetur. Lorem ipsum dolor sit<sup>abc </sup> **<sup>123</sup>** amet consectetur.

Example, Interior italic: Lorem ipsum dolor sit<sub>abc </sub> *<sub>123</sub>* amet consectetur. Lorem ipsum dolor sit<sup>abc </sup> *<sup>123</sup>* amet consectetur.

Example, Links in scripts: Lorem ipsum dolor sit[<sub>abc 123</sub>](https://mit.edu) amet consectetur. Lorem ipsum dolor sit[<sup>abc 123</sup>](https://mit.edu) amet consectetur.

Example, Scripts in Links: Lorem ipsum dolor [sit<sub>abc 123</sub> amet](https://mit.edu) consectetur. Lorem ipsum dolor [sit<sup>abc 123</sup> amet](https://mit.edu) amet consectetur.

Example, Resource Links in scripts: Lorem ipsum dolor sit{{% resource_link "d8b66928-ee87-4b59-ac37-d78f781e73e6" "<sub>abc 123</sub>" %}} amet consectetur. Lorem ipsum dolor sit{{% resource_link "d8b66928-ee87-4b59-ac37-d78f781e73e6" "<sup>abc 123</sup>" %}} amet consectetur.

Example, Scripts in Resource Links: Lorem ipsum dolor {{% resource_link "d8b66928-ee87-4b59-ac37-d78f781e73e6" "sit<sub>abc 123</sub> amet" %}} consectetur. Lorem ipsum dolor {{% resource_link "d8b66928-ee87-4b59-ac37-d78f781e73e6" "sit<sup>abc 123</sup> amet" %}} consectetur.

### Usage in tables

{{< tableopen >}}{{< theadopen >}}{{< tropen >}}{{< thopen >}}
Header One
{{< thclose >}}{{< thopen >}}
Header Two
{{< thclose >}}{{< thopen >}}
Header Three
{{< thclose >}}{{< trclose >}}{{< theadclose >}}{{< tbodyopen >}}{{< tropen >}}{{< tdopen >}}
lorem<sub>abc 123</sub> ipsum
{{< tdclose >}}{{< tdopen >}}
lorem[<sup>†</sup>](https://mit.edu) ipsum
{{< tdclose >}}{{< tdopen >}}
lorem{{% resource_link "d8b66928-ee87-4b59-ac37-d78f781e73e6" "<sup>‡</sup>" %}} ipsum
{{< tdclose >}}{{< trclose >}}{{< tropen >}}{{< tdopen >}}
a
{{< tdclose >}}{{< tdopen >}}
b
{{< tdclose >}}{{< tdopen >}}
c
{{< tdclose >}}{{< trclose >}}{{< tbodyclose >}}{{< tableclose >}}