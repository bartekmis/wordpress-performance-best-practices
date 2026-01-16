# Sections

---

## 1. Database Optimization (db)

**Impact:** CRITICAL
**Description:** Database queries are the primary bottleneck in WordPress performance. Unoptimized queries, missing indexes, direct database access, and improper use of WP_Query can cause severe slowdowns, especially on high-traffic sites. Following WordPress VIP standards for database operations is essential for scalable applications.

## 2. Caching Strategies (cache)

**Impact:** CRITICAL
**Description:** Effective caching reduces server load by avoiding redundant computations and database queries. Understanding when to use transients vs object cache, implementing proper cache invalidation, and leveraging page caching are fundamental to WordPress performance optimization.

## 3. Asset Management (asset)

**Impact:** HIGH
**Description:** How scripts and styles are loaded directly affects page load time and Core Web Vitals. Proper enqueueing, conditional loading, defer/async attributes, and avoiding render-blocking resources are key to frontend performance.

## 4. Theme Performance (theme)

**Impact:** HIGH
**Description:** Theme code executes on every page load. Avoiding queries in templates, using proper template hierarchy, optimizing loops, and following WordPress template best practices prevent performance degradation at the presentation layer.

## 5. Plugin Architecture (plugin)

**Impact:** MEDIUM-HIGH
**Description:** Well-architected plugins load efficiently and don't impact performance when not needed. Proper hook usage, conditional loading, autoloading, and following WordPress plugin standards ensure plugins scale with site growth.

## 6. Media Optimization (media)

**Impact:** MEDIUM
**Description:** Images and media often account for the majority of page weight. Proper image sizing, lazy loading, responsive images, and leveraging WordPress's built-in media handling improve load times and user experience.

## 7. API and AJAX (api)

**Impact:** MEDIUM
**Description:** REST API and AJAX requests require careful optimization. Proper endpoint design, response caching, nonce handling, and avoiding admin-ajax bottlenecks are essential for interactive WordPress applications.

## 8. Advanced Patterns (advanced)

**Impact:** LOW-MEDIUM
**Description:** Advanced optimization techniques for high-traffic sites including autoload optimization, WP-Cron management, memory management, and platform-specific optimizations used by enterprise WordPress hosts.
