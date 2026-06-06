# Voyara — Quarto Website

A multi-page Quarto website for a travel agency offering tour planning, visa
assistance, flight tickets, and study-abroad services.

## Pages
- `index.qmd` — Home (hero, services, stats, featured tours, process, CTA)
- `services.qmd` — Full service list
- `tours.qmd` — Sample tour packages
- `study.qmd` — Study-abroad services & destinations
- `about.qmd` — About the company
- `contact.qmd` — Inquiry form + contact details

## Requirements
Install Quarto (one time): https://quarto.org/docs/get-started/

## Preview locally (live reload)
```bash
cd voyara
quarto preview
```
Opens at http://localhost:port with auto-refresh as you edit.

## Build the static site
```bash
cd voyara
quarto render
```
Output goes to the `_site/` folder — a complete static site you can host
anywhere (Netlify, GitHub Pages, Vercel, any web server).

## Customize
- Colors & fonts: `assets/css/voyara.scss` (Voyara palette + Fraunces/Outfit fonts)
- Component styles: `assets/css/extra.css`
- Logo: `assets/img/logo.svg`
- Navigation & site title: `_quarto.yml`

## Make the contact form work
The form in `contact.qmd` is a front-end demo. To receive submissions, point it
at a service like Formspree, Basin, or your own endpoint, or embed a Google Form.

## Deploy to GitHub Pages (quick)
```bash
quarto publish gh-pages
```
