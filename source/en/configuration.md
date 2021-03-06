---
title: Config Reference
---

**Valine** Supports two different initialization methods:
```html
<!-- Write the argument in the constructor -->
<script>
    new Valine({
        el:'#vcomment',
        appId:'<APP_ID>',
        appKey:'<APP_KEY>'
    })
</script>

<!-- or Call the init method -->
<script>
    var valine = new Valine();
    valine.init({
        el:'#vcomment',
        appId:'<APP_ID>',
        appKey:'<APP_KEY>'
    })
</script>
```

## el
- Type:`String`
- Default:`null`
- Required:`true`

The DOM element to be mounted on initialization. It can be a CSS selector string or an actual HTMLElement.

## appId
- Type:`String`
- Default:`null`
- Required:`true`

Application `<APP_ID>` from `Leancloud`.

## appKey
- Type:`String`
- Default:`null`
- Required:`true`

Application `<APP_KEY>` from `Leancloud`.

## <del>region</del>
- Type:`String`
- Default:`cn`
- Required:`false`

Storage node.

> Leancloud sdk removed the region option in `v3.8.0`:  
>  [leancloud/javascript-sdk/releases/tag/v3.8.0](https://github.com/leancloud/javascript-sdk/releases/tag/v3.8.0)

Optional value:

- `cn` - Chinese mainland node
- `us` - Overseas node

## placeholder
- Type:`String`
- Default:`null`
- Required:`false`

Comment box placeholders.

## notify
- Type:`Boolean`
- Default:`false`
- Required:`false`

Mail notifier, Please refer to the [configuration](https://github.com/xCss/Valine/wiki/Valine-%E8%AF%84%E8%AE%BA%E7%B3%BB%E7%BB%9F%E4%B8%AD%E7%9A%84%E9%82%AE%E4%BB%B6%E6%8F%90%E9%86%92%E8%AE%BE%E7%BD%AE).


## verify
- Type:`Boolean`
- Default:`false`
- Required:`false`

Validation code.

## path
- Type:`String`
- Default:`window.location.pathname`
- Required:`false`

Article path(just like duoshuo `thread`).

Optional value:
- `window.location.pathname` (recommend)
- `window.location.href`
- customize (`Please ensure uniqueness`)

## avatar
- Type:`String`
- Default:`mm`
- Required:`false`

`Gravatar` type. 

Optional value:
- `''`(Empty string)
- `mp`
- `identicon`
- `monsterid`
- `wavatar`
- `retro`
- `robohash`
- `hide` 

See the [Avatar setting](/en/avatar.html) for more details.


## meta
- Type:`Array`
- Default:`['nick','mail','link']`
- Required:`false`

Reviewer attributes.

## pageSize
- Type:`Number`
- Default:`10`
- Required:`false`

Number of pages per page.


## lang
- Type:`String`
- Default:`zh-cn`
- Required:`false`

Multilingual support.

Optional value：
- `zh-cn`
- `en`

If you need a custom language, please refer to [i18n](/en/i18n.html)。


## visitor
- Type:`Boolean`
- Default:`false`
- Required:`false`

[Article reading statistics](/en/visitor.html).


## highlight
- Type:`Boolean`
- Default:`true`
- Required:`false`

`Code highlighting`, it's enabled by default, please close it selectively.

## avatarForce
- Type:`Boolean`
- Default:`false`
- Required:`false`
  
Each time you access `forced` pulls the latest avatar.

## recordIP
- Type:`Boolean`
- Default:`false`
- Required:`false`

Record reviewer IP.

> `v1.3.5+`
