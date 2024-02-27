---
layout: page
title: Playwright E2E results
permalink: /playwright/
traceviewerurl: https://trace.playwright.dev/?trace=https://graywolfcorp.github.io/trace-files/
---


<table>
{% for test in site.data.test-results.tests %}
    <tr>
        <td>
            <a target="_blank" href="{{page.traceviewerurl}}{{ test.name }}"  >{{ test.name }}</a>
        </td>
        <td>
            {{ test.date}}
        </td>
        <td>
            {{ test.size}}
        </td>
    </tr>
{% endfor %}
</table>


[trace-playwright]: https://trace.playwright.dev/?trace=https://graywolfcorp.github.io/trace-files/
