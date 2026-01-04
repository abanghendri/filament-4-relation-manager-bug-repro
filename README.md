# Filament 4 Relationship Manager Bug Reproduction

This repository reproduces an issue where relationship managers in Filament 4.0 show the parent table instead of related records.

## Steps to Reproduce
1. Clone repository
2. Run `composer install`
3. Set up `.env` file with database
4. Run migrations and seeders
5. Visit `/admin/questions`
6. Click on any question to view details
7. **Expected**: See related Options table
8. **Actual**: See parent Questions table again

## Environment
- Laravel: 12.x
- Filament: 4.0
- PHP: 8.3