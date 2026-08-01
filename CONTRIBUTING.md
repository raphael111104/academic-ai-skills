# Panduan Kontribusi

Terima kasih telah berminat untuk berkontribusi pada **Academic & Critical AI Agent Skills Repository**!

## Cara Berkontribusi

1. **Fork** repositori ini.
2. Buat branch baru untuk fitur atau skill baru:
   ```bash
   git checkout -b feature/nama-skill-baru
   ```
3. Tambahkan folder skill baru di bawah direktori `skills/` dengan struktur wajib:
   ```
   skills/nama-skill-baru/
   └── SKILL.md
   ```
4. Pastikan `SKILL.md` memiliki YAML Frontmatter yang valid (`name` dan `description`).
5. Commit perubahan Anda dan buat **Pull Request**.

## Standar Penulisan Skill
- Gunakan bahasa yang jelas, profesional, dan imperatif.
- Sertakan konteks pemicu (*When to Use*), panduan langkah demi langkah, dan potensi kesalahan (*Gotchas*).
- Hindari klaim berlebihan dan jaga standar akademis yang objektif.
