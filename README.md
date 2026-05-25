# DashboardKit — React Admin Dashboard

A free React admin dashboard template built with React 18, Vite, and Bootstrap 5. Includes a Sales dashboard, UI element pages, icon libraries, and authentication pages.

---

## Tech Stack

| Package | Version |
|---------|---------|
| React | ^18.3.1 |
| React DOM | ^18.3.1 |
| Vite | ^5.4.1 |
| Bootstrap | 5.3.3 |
| React Bootstrap | ^2.10.4 |
| React Router DOM | ^6.26.1 |
| ApexCharts | ^4.3.0 |
| react-apexcharts | ^1.7.0 |
| styled-components | ^6.1.13 |
| simplebar-react | ^3.2.6 |
| feather-icons-react | ^0.7.0 |
| lodash-es | ^4.17.21 |
| yup | ^1.4.0 |
| web-vitals | ^4.2.3 |
| Package Manager | yarn 4.6.0 |

---

## Getting Started

### Install

```bash
yarn install
```

### Run Dev Server

```bash
yarn start
```

### Build

```bash
yarn build
```

### Preview

```bash
yarn preview
```

### Lint

```bash
yarn lint
yarn lint:fix
```

### Format

```bash
yarn prettier
```

### Deploy (GitHub Pages)

```bash
yarn deploy
```

---

## Project Structure

```
src/
├── App.jsx                          # Root — sets up RouterProvider
├── index.jsx                        # Entry point
├── index.scss                       # Global SCSS entry
├── menu-items.js                    # Sidebar navigation config (flat layout)
├── menu-items-collapse.js           # Sidebar navigation config (collapse layout)
├── routes/
│   ├── index.jsx                    # Router setup
│   └── MainRoutes.jsx               # Protected/main routes
├── layouts/
│   ├── AdminLayout/                 # Main admin shell
│   │   ├── index.jsx
│   │   ├── Breadcrumb/
│   │   ├── NavBar/                  # Top navbar (left + right slots)
│   │   ├── Navigation/              # Sidebar with NavItem, NavGroup, NavCollapse, NavIcon
│   │   └── MobileHeader/
│   └── GuestLayout/                 # Layout for login/register
├── views/
│   ├── auth/
│   │   ├── login.jsx
│   │   └── register.jsx
│   ├── dashboard/
│   │   └── DashSales/
│   │       ├── index.jsx            # Sales dashboard view
│   │       └── chart/
│   │           ├── sales-account-chart.js
│   │           ├── sales-customer-satisfication-chart.js
│   │           ├── sales-support-chart.js
│   │           └── sales-support-chart1.js
│   ├── sample/index.jsx
│   └── ui-elements/
│       ├── basic/
│       │   ├── BasicColor.jsx
│       │   └── BasicTypography.jsx
│       └── icons/
│           ├── Feather.jsx
│           ├── FontAwesome.jsx
│           └── Material.jsx
├── components/
│   ├── Card/MainCard.jsx
│   ├── Loader/                      # Bar, Container, Loader, Progress, Spinner
│   └── Widgets/
│       ├── FeedTable.jsx
│       ├── ProductTable.jsx
│       └── Statistic/
│           ├── FlatCard.jsx
│           └── ProductCard.jsx
├── contexts/ConfigContext.jsx
├── hooks/useWindowSize.js
├── store/actions.js
├── config/constant.js
├── data/
│   ├── feedData.js
│   └── productTableData.jsx
├── utils/getImageUrl.js
└── assets/
    ├── fonts/                       # Inter, Feather, FontAwesome, Material, Cryptocoins
    ├── images/                      # Logo, user avatars, widget images
    └── scss/                        # Theming, component styles, layout styles
```

---

## Dashboard — Sales View (`/dashboard/sales`)

Stat cards displayed: Customers, Revenue, Growth, Returns, Downloads, Order.

Charts:
- **Conversion Rate** — bar/area chart (53.94%)
- **Order Delivered** — bar chart with monthly breakdown
- **Department-wise Monthly Sales Report** — line/area chart ($21,356.46 total sales)
- **Customer Satisfaction** — pie chart

Tables:
- **Product Table** — product listing with data
- **Feed Table** — activity feed

Product stat cards: Total Profit, Total Orders, Average Price, Product Sold.

---

## Sidebar Navigation

**Navigation group**
- Dashboard → Sales

**Elements group**
- Typography
- Color
- Icons → Feather / Font Awesome / Material

**Pages group**
- Login
- Register

---

## Icon Libraries

Three icon sets are available via dedicated pages:

- **Feather Icons** (`/icons/Feather`)
- **Font Awesome 5** (`/icons/font-awesome-5`)
- **Material Icons** (`/icons/material`)

---

## CI/CD

GitHub Actions workflows are included:

- `.github/workflows/bootstrap-prod.yml` — Bootstrap production build
- `.github/workflows/react-prod.yml` — React production build

---

## License

Design and code by [CodedThemes](https://www.codedthemes.com). Licensed under MIT. Distributed by [ThemeWagon](https://themewagon.com).
