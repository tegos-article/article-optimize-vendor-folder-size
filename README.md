# Optimize Vendor Folder Size

![Optimize Vendor Folder Size](assets/poster.jpg)

This article provides a practical guide to reducing the size of the `vendor/` folder in PHP/Laravel projects.
By addressing bloated dependencies, you can achieve faster deployments, smaller Docker images, and lower storage costs.
The steps include auditing the vendor folder, trimming unnecessary SDK components, removing test fixtures, moving dev
tools to `require-dev`, and pruning unused packages. The result? A 40% reduction in vendor folder size (from 281 MB to
119.8 MB), leading to quicker CI/CD pipelines and optimized resource usage.

**Quick recap:**

- Use `du -h` to identify large dependencies.
- Limit SDKs like AWS to only required services (e.g., S3).
- Request package maintainers to exclude test data in production dists.
- Move dev tools (e.g., Telescope, Clockwork) to `require-dev`.
- Regularly audit and remove unused packages.

Check the full article for detailed steps and examples to slim down your `vendor/` folder today!

🔗 **Read the article**: [Optimize Vendor Folder Size](https://dev.to/tegos/optimize-vendor-folder-size-1m01)