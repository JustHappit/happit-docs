# Data transfer: Statistics

```javascript
{
    users: {
        active: number,
        total: number
    },
    hotspots: {
        opened: number,
        mostViewed: [{
            views: number,
            uniqueId: string
        }],
        leastViewed: [{
            views: number,
            uniqueId: string
        }]
    },
    savings: number
}
```
