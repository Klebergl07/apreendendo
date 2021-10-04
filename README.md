// TODO: Build a Tile.
override fun onTileRequest(requestParams: TileRequest) = serviceScope.future {

    Tile.builder()
        // If there are any graphics/images defined in the Tile's layout, the system will
        // retrieve them using onResourcesRequest() and match them with this version number.
        .setResourcesVersion(RESOURCES_VERSION)

        // Creates a timeline to hold one or more tile entries for a specific time periods.
        .setTimeline(
            Timeline.builder().addTimelineEntry(
                TimelineEntry.builder().setLayout(
                    Layout.builder().setRoot(
                        Text.builder().setText("Hello, world!")
// TODO: Review creation of Tile for Preview.
tileManager = TileManager(
    context = this,
    component = ComponentName(this, GoalsTileService::class.java),
    parentView = rootLayout
)
tileManager.create()
