# Model

## Defining Model

`php artisan make:model Flight --migration`

## Eloquent Model Convention

```php
// Flight.php

<?php

namespace App;

use Illuminate\Database\Eloquent\Model;

class Flight extends Model
{
    /**
     * Custom names of the timestamps columns
     *
     * @var string
     * @var string
     * /
    const CREATED_AT = 'creation_date';
    const UPDATED_AT = 'last_update';

    /**
     * The connection name for the model.
     *
     * @var string
     */
    protected $connection = 'connection-name';

    // By default, the snake_case, plural name of the class
    // will be use as the table name.
    /**
     * The table associated with the model.
     *
     * @var string
     */
    protected $table = 'my_flights';

    // By default, the primary key column will be named "id".
    /**
     * The primary key associated with the table.
     *
     * @var string
     */
    protected $primaryKey = 'flight_id';

    // To use a non-incrementing or a non-numeric primary key.
    /**
     * Indicates if the IDs are auto-incrementing.
     *
     * @var bool
     */
    public $incrementing = false;

    /**
     * The "type" of the auto-incrementing ID.
     *
     * @var string
     */
    protected $keyType = 'string';

    /**
     * Indicates if the model should be timestamped.
     *
     * @var bool
     */
    public $timestamps = false;

    /**
     * The storage format of the model's date columns.
     *
     * @var string
     */
    protected $dateFormat = 'U';

    /**
     * The model's default values for attributes.
     *
     * @var array
     */
    protected $attributes = [
        'delayed' => false,
    ];

    /**
     * The attributes that should be cast to native types.
     *
     * @var array
     */
    protected $casts = [
        'options' => 'array',
    ];
}
```

Reference: https://laravel.com/docs/7.x/eloquent#eloquent-model-conventions
