# Data transfer: Happspots and sequences

## Happspot

```javascript
{
    uniqueId: string,
    sequenceId: number,
    sequenceOrdinal: number,
    status: number,
    url: string,
    target: object,
    offsetTop: number,
    offsetLeft: number,
    isRead: boolean,
    activityId: number,

    versions: {
        published/draft: {
            id: number,
            uniqueId: string,
            hotspotId: number,
            type: number,
            title: object,
            calloutContent: object,
            color: string,
            isAutoOpen: boolean,
            isPinned: boolean,
            calloutOrigin: string,
            width: number
        }
    }

    //
    // deprecated properties
    //
    id: number
}
```

## Sequence

```javascript
{
    uniqueId: string,
    name: string,
    createdOn: date,
    modifiedOn: date,
    isRead: boolean,
    isGlobal: boolean,
    hotspots: string[],

    //
    // deprecated properties
    //
    id: number
}
```