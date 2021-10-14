# Prototype for usability testing of new service design

Built with [Eleventy](https://www.11ty.dev/).

## Setup

1. Move to the project directory e.g. `cd prototype-service`.
2. Run `npm install`.
3. Run `npx @11ty/eleventy --serve --port=8081`.
4. Go to http://localhost:8081/london-supported-lodgings-service/

## Architecture

The site is using the nunjucks templating languange, so template files have a .njk extension.

Components are in \_includes/components. Save them there, with CSS in a `<style>` element if necessary above the HTML. To include the components in the page use the nunjucks include syntax: `{% include './_includes/components/breadcrumb.njk' %}`.

The page content is added to the HTML in \_includes/layout.njk through `{{ content | safe }}`.
