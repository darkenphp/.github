```
 ____             _              
|  _ \  __ _ _ __| | _____ _ __  
| | | |/ _` | '__| |/ / _ \ '_ \ 
| |_| | (_| | |  |   <  __/ | | |
|____/ \__,_|_|  |_|\_\___|_| |_|
```

A PHP framework with a twist—think Nuxt.js and Astro had a PHP baby, but without the node_modules drama, npm meltdowns. Composer? We’re cool with that; it’s the classy uncle we all respect. We’ve got components with slots (because who doesn’t love a good slot?), and every method, property, and class is IDE auto-completion-friendly—no guessing games here!

Auto-magic? Nope, we’re not wizards. Darken needs to compile while you work your magic or at least once before you hit deploy. Oh, and when you create a new project, you won’t be greeted by a junk drawer of files and folders—just the bare essentials, like a tidy minimalist's dream.

```php
<?php
$page = new class {

    #[\Darken\Attributes\RouteParam]
    public string $name;

    public function getGreeting(): string
    {
        return 'Hello, ' . ucfirst($this->name) . '!';
    }
};
?>
<h1><?= $page->getGreeting(); ?></h1>
```
