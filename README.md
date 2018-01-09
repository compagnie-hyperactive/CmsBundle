cms bundle presentation

# Instalation
## Site Entity
Create a entity extending the `Lch\CmsBundle\Entity\Site`

The minimum entity have to be
```php
<?php

namespace ExempleBundle\Entity;

use Doctrine\ORM\Mapping as ORM;
use Lch\CmsBundle\Entity\Site as BaseSite;

/**
 * Class Site
 * @package AppBundle\Entity
 *
 * @ORM\Table(name="site")
 * @ORM\Entity()
 */
class Site extends BaseSite
{
    /**
     * @var int
     *
     * @ORM\Column(name="id", type="integer")
     * @ORM\Id
     * @ORM\GeneratedValue(strategy="AUTO")
     */
    private $id;
}
```
