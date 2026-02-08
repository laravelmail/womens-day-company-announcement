# Womens Day Company Announcement

A professional announcement celebrating International Women's Day and highlighting the company's commitment to gender equality, women's empowerment, and diversity in Education and Business.

![Thumbnail](./thumbnail.png)

## Template Details

- **Industries:** Women's Empowerment in Education,  Business & Professional Services
- **Message Type:** Newsletter
- **Tags:** celebration, empowerment, inclusion, diversity, womensday

## Files
- `index.html`: The improved, localized, and branded HTML template.
- `template.blade.php`: Ready-to-use Laravel Blade template with `asset()` helpers.
- `assets/`: Directory containing localized images and styles used in the template.

## Usage in Laravel

### 1. Store the Template
Place the `index.html` content in a Blade view (e.g., `resources/views/emails/womens-day-company-announcement.blade.php`).

### 2. Handle Assets
Move the content of `assets/` to your public directory (e.g., `public/vendor/mail-templates/womens-day-company-announcement/`) and update the paths in the HTML to use the `asset()` helper.

### 3. Send Email
```php
Mail::to($user)->send(new \App\Mail\GenericEmail([
    'view' => 'emails.womens-day-company-announcement',
    'data' => [
        // Your dynamic data here
    ]
]));
```

---
*Created with ❤️ by **[LaravelMail.com](https://laravelmail.com)** - Your source for professional email templates.*
