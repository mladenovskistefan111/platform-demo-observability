# Dashboards

One dashboard per service, provisioned from `grafana/provisioning/dashboards/`. Each carries the tag of its service, which
is how the portal finds it (`grafana/dashboard-selector: tags @> '<tag>'`).

| Dashboard | uid | Link |
|---|---|---|
| Ad Service | `ad-service-overview` | [open](https://grafana.platform-demo.test/d/ad-service-overview) |
| Cart Service | `cart-service-overview` | [open](https://grafana.platform-demo.test/d/cart-service-overview) |
| Checkout Service | `checkout-service-overview` | [open](https://grafana.platform-demo.test/d/checkout-service-overview) |
| Currency Service | `currency-service-overview` | [open](https://grafana.platform-demo.test/d/currency-service-overview) |
| Email Service | `email-service-overview` | [open](https://grafana.platform-demo.test/d/email-service-overview) |
| Frontend Service | `frontend-overview` | [open](https://grafana.platform-demo.test/d/frontend-overview) |
| Payment Service | `payment-service-overview` | [open](https://grafana.platform-demo.test/d/payment-service-overview) |
| Product Catalog Service | `product-catalog-overview` | [open](https://grafana.platform-demo.test/d/product-catalog-overview) |
| Recommendation Service | `recommendation-service-overview` | [open](https://grafana.platform-demo.test/d/recommendation-service-overview) |
| Shipping Service | `shipping-service-overview` | [open](https://grafana.platform-demo.test/d/shipping-service-overview) |

All 198 dashboard queries were run against a live stack; 186 return data and the remaining 12 are error-rate and
status-code panels that are empty simply because nothing failed.
