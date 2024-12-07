Note: This is an official and reasonably maintained fork of the popular https://github.com/dingo/api repository by one of the maintainers of that project. The reason it was forked is due to broken integrations with CI tools such as travis (which can only be fixed by owner), and in general to be able to better support the project and ensure non-breaking updates.

In order to move to this repo, you merely need to update your composer file. All the namespaces and other aspects of the project are the same. Example instructions are below, to use the latest version:

```bash
composer remove dingo/api
composer require api-ecosystem-for-laravel/dingo-api
```

Please note, we do not actively maintain the Lumen support of this project. If you are still using Lumen, we recommend you migrate to Laravel.

---

## Dingo API: Spesialis API RESTful untuk Laravel

**Benar sekali!** Dingo API adalah sebuah paket Laravel yang sangat populer dan kuat untuk membangun API RESTful yang skalabel dan mudah dikelola. Dingo dirancang khusus untuk memberikan fitur-fitur yang diperlukan untuk mengembangkan API yang modern dan efisien.

### Apa itu Dingo API?

Dingo API adalah sebuah lapisan abstraksi di atas Laravel HTTP kernel yang menyediakan fitur-fitur tambahan seperti:

* **Routing fleksibel:** Dingo memungkinkan Anda mendefinisikan rute API secara terpisah dari rute web aplikasi Anda.
* **Versi API:** Anda dapat dengan mudah mengelola berbagai versi API Anda.
* **Transformasi respons:** Dingo menyediakan cara mudah untuk mengubah data sebelum dikirim ke klien.
* **Otentikasi:** Dingo mendukung berbagai mekanisme otentikasi seperti token, OAuth, dan lainnya.
* **Dokumentasi otomatis:** Dingo dapat secara otomatis menghasilkan dokumentasi API Anda.
* **Middleware:** Anda dapat menggunakan middleware untuk melakukan tindakan sebelum dan sesudah permintaan API diproses.
* **Exceptions:** Dingo menyediakan mekanisme penanganan pengecualian yang khusus untuk API.

### Kenapa Menggunakan Dingo API?

* **Struktur yang jelas:** Dingo membantu Anda menjaga struktur API Anda tetap bersih dan terorganisir.
* **Fitur lengkap:** Dingo menyediakan semua fitur yang Anda butuhkan untuk membangun API yang kuat.
* **Komunitas yang aktif:** Dingo memiliki komunitas yang besar dan aktif, sehingga Anda dapat dengan mudah menemukan bantuan jika Anda mengalami masalah.
* **Integrasi dengan Laravel:** Dingo terintegrasi dengan baik dengan ekosistem Laravel, sehingga Anda dapat memanfaatkan semua fitur yang ditawarkan oleh Laravel.

### Contoh Penggunaan Sederhana

```php
use Dingo\Api\Routing\Router;

$api = app(Router::class);

$api->version('v1', function (Router $api) {
    $api->get('users', 'App\Http\Controllers\UserController@index');
});
```

Kode di atas mendefinisikan sebuah rute API versi 1 untuk mendapatkan daftar pengguna.

### Kapan Harus Menggunakan Dingo API?

Anda sebaiknya mempertimbangkan untuk menggunakan Dingo API jika:

* Anda ingin membangun API RESTful yang kompleks dan skalabel.
* Anda membutuhkan fitur-fitur tambahan seperti versi API, transformasi respons, dan otentikasi yang lebih fleksibel.
* Anda ingin memiliki kontrol penuh atas struktur API Anda.

### Kesimpulan

Dingo API adalah pilihan yang sangat baik untuk membangun API RESTful di Laravel. Dengan fitur-fitur yang lengkap dan komunitas yang aktif, Dingo dapat membantu Anda membangun API yang berkualitas tinggi dan efisien.

**Apakah Anda ingin mempelajari lebih lanjut tentang fitur-fitur spesifik Dingo API atau bagaimana cara menginstal dan mengkonfigurasinya?**

**Beberapa topik yang mungkin menarik untuk dibahas lebih lanjut:**

* **Membuat versi API**
* **Menerapkan otentikasi**
* **Menyusun respons API**
* **Menangani kesalahan**
* **Menguji API**

Jangan ragu untuk bertanya!


---

![](https://cloud.githubusercontent.com/assets/829059/9216039/82be51cc-40f6-11e5-88f5-f0cbd07bcc39.png)

The Dingo API package is meant to provide you, the developer, with a set of tools to help you easily and quickly build your own API. While the goal of this package is to remain as flexible as possible it still won't cover all situations and solve all problems.

[![CI Tests](https://github.com/api-ecosystem-for-laravel/dingo-api/actions/workflows/ci.yml/badge.svg?branch=master)](https://github.com/api-ecosystem-for-laravel/dingo-api/actions)
[![License](https://img.shields.io/packagist/l/api-ecosystem-for-laravel/dingo-api.svg?style=flat-square)](LICENSE)
[![Development Version](https://img.shields.io/packagist/vpre/api-ecosystem-for-laravel/dingo-api.svg?style=flat-square)](https://packagist.org/packages/api-ecosystem-for-laravel/dingo-api)
[![Monthly Installs](https://img.shields.io/packagist/dm/api-ecosystem-for-laravel/dingo-api.svg?style=flat-square)](https://packagist.org/packages/api-ecosystem-for-laravel/dingo-api)

## Features

This package provides tools for the following, and more:

- Content Negotiation
- Multiple Authentication Adapters
- API Versioning
- Rate Limiting
- Response Transformers and Formatters
- Error and Exception Handling
- Internal Requests
- API Blueprint Documentation

## Documentation

Please refer to our extensive [Wiki documentation](https://github.com/api-ecosystem-for-laravel/dingo-api/wiki) for more information.

## API Boilerplate

If you are looking to start a new project from scratch, consider using the [Laravel API Boilerplate](https://github.com/specialtactics/laravel-api-boilerplate), which builds on top of the dingo-api package, and adds a lot of great features for API development.

## Support

For answers you may not find in the Wiki, avoid posting issues. Feel free to ask for support on the dedicated [Slack](https://larachat.slack.com/messages/api/) room. Make sure to mention **specialtactics** so he is notified.

Alternatively, you can start a [new discussion in the Q&A category](https://github.com/api-ecosystem-for-laravel/dingo-api/discussions/categories/q-a).

## License

This package is licensed under the [BSD 3-Clause license](http://opensource.org/licenses/BSD-3-Clause).
