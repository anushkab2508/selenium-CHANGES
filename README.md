# selenium-CHANGES

# Replacements for Deprecated WebDriver Locator Methods
Selenium 4.3.0
* Deprecated find_element_by_* and find_elements_by_* are now removed (#10712)
* Deprecated Opera support has been removed (#10630)
* Fully upgraded from python 2x to 3.7 syntax and features (#10647)
* Added a devtools version fallback mechanism to look for an older version when mismatch occurs (#10749)
* Better support for co-operative multi inheritance by utilising super() throughout
* Improved type hints throughout

## Using id:

Replace:

```python
element = find_element_by_id("element_id")
```
with:

```python
element = driver.find_element(By.ID, "element_id")
```

## Using name:

Replace:

```python
element = find_element_by_name("element_name")
```
with:

```python
element = driver.find_element(By.NAME, "element_name")
```

## Using link text:

Replace:

```python
element = find_element_by_link_text("element_link_text")
```
with:

```python
element = driver.find_element(By.LINK_TEXT, "element_link_text")
```

## Using partial link text:

Replace:

```python
element = find_element_by_partial_link_text("element_partial_link_text")
```
with:

```python
element = driver.find_element(By.PARTIAL_LINK_TEXT, "element_partial_link_text")
```

## Using tag name:

Replace:

```python
element = find_element_by_tag_name("element_tag_name")
```
with:

```python
element = driver.find_element(By.TAG_NAME, "element_tag_name")
```

## Using CSS selector:

Replace:

```python
element = find_element_by_css_selector("element_css_selector")
```
with:

```python
element = driver.find_element(By.CSS_SELECTOR, "element_css_selector")
```

## Using Xpath:

Replace:

```python
element = find_element_by_xpath("element_xpath")
```
with:

```python
element = driver.find_element(By.XPATH, "element_xpath")
```
