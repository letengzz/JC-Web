# 常见的 DOCTYPE 声明

## `HTML 5`

```html
<!DOCTYPE html>
```

## `HTML 4.01 Strict`

这个`DTD`包含所有 `HTML` 元素和属性，但不包括表象或过时的元素(如`font`)。框架集是不允许的。

```
<!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 4.01//EN" "http://www.w3.org/TR/html4/strict.dtd">
```

## `HTML 4.01 Transitional`

这个 `DTD` 包含所有 `HTML` 元素和属性，包括表象或过时的元素(如 `font`)。框架集是不允许的。

```html
<!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 4.01 Transitional//EN" "http://www.w3.org/TR/html4/loose.dtd">
```

## `HTML 4.01 Frameset`

这个 `DTD` 与 `HTML 4.01 Transitional` 相同，但是允许使用框架集内容。

```
<!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 4.01 Frameset//EN" "http://www.w3.org/TR/html4/frameset.dtd">
```

## `XHTML 1.0 Strict`

这个 `DTD` 包含所有 `HTML` 元素和属性，但不包括表象或过时的元素(如 `font`)。框架集是不允许的。结构必须按标准格式的 `XML` 进行书写。

```html
<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Strict//EN" "http://www.w3.org/TR/xhtml1/DTD/xhtml1-strict.dtd">
```

## `XHTML 1.0 Transitional`

这个 `DTD` 包含所有 `HTML` 元素和属性，包括表象或过时的元素(如 `font` )。框架集是不允许的。结构必须按标准格式的 `XML` 进行书写。

```html
<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Transitional//EN" "http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">
```

## `XHTML 1.0 Frameset`

这个`DTD`与`XHTML 1.0 Transitional`相同，但是允许使用框架集内容。

```html
<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Frameset//EN" "http://www.w3.org/TR/xhtml1/DTD/xhtml1-frameset.dtd">
```

## `XHTML 1.1`

这个`DTD`与`XHTML 1.0 Strict`相同，但是允许您添加模块（例如为东亚语言提供 `ruby` 支持）。

```html
<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.1//EN" "http://www.w3.org/TR/xhtml11/DTD/xhtml11.dtd">
```

