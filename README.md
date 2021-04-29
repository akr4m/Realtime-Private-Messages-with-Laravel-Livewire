## Realtime Private Messages with Laravel Livewire

Demo Project of Realtime Private Messages with Laravel Livewire

### Web Routes

```php
<?php

use Illuminate\Support\Facades\Route;

Route::get('/', function () {
    return view('welcome');
});

Auth::routes();

Route::get('/home', 'HomeController@index')->name('home');

Route::get('/conversations', 'Conversations\ConversationController@index')->name('conversations.index');
Route::get('/conversations/create', 'Conversations\ConversationController@create')->name('conversations.create');
Route::get('/conversations/{conversation}', 'Conversations\ConversationController@show')->name('conversations.show');

```
