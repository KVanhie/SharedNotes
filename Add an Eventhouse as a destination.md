#study #azure/fabric  #azure/fabric/eventhouse

[Source](https://learn.microsoft.com/en-us/fabric/real-time-intelligence/event-streams/add-destination-kql-database?pivots=enhanced-capabilities)

# Direct ingestion mode

1. In **Edit mode** for your eventstream, select **Add destination** on the ribbon or select the **Transform events or add destination** card on the canvas, and then select **Eventhouse**.
    
    [![A screenshot of selecting Eventhouse in the Add destination dropdown list.](https://learn.microsoft.com/en-us/fabric/real-time-intelligence/event-streams/media/add-destination-kql-database/add-eventhouse-destination.png)](https://learn.microsoft.com/en-us/fabric/real-time-intelligence/event-streams/media/add-destination-kql-database/add-eventhouse-destination.png#lightbox)
    
2. On the Eventhouse screen, select **Direct ingestion**.
    
3. Enter a **Destination name**, a **Workspace**, and an **Eventhouse** from the selected workspace.
    
4. Select **Save**.
    
    ![A screenshot of the Eventhouse configuration screen.](https://learn.microsoft.com/en-us/fabric/real-time-intelligence/event-streams/media/add-destination-kql-database/eventhouse-direct-ingestion.png)
    
5. Connect the new Eventhouse destination card to the output of your eventstream if not already connected, and then select **Publish**.
    
    [![A screenshot of the eventstream with the Publish button highlighted.](https://learn.microsoft.com/en-us/fabric/real-time-intelligence/event-streams/media/add-destination-kql-database/edit-mode.png)](https://learn.microsoft.com/en-us/fabric/real-time-intelligence/event-streams/media/add-destination-kql-database/edit-mode.png#lightbox)
    
6. In **Live view**, select **Configure** in the Eventhouse destination node.
    
    [![A screenshot of the published eventstream with the Configure button in the KQL Database destination highlighted.](https://learn.microsoft.com/en-us/fabric/real-time-intelligence/event-streams/media/add-destination-kql-database/live-view.png)](https://learn.microsoft.com/en-us/fabric/real-time-intelligence/event-streams/media/add-destination-kql-database/live-view.png#lightbox)
    
7. Your Eventhouse opens in the **Get data** screen. Select an existing table of the KQL database, or select **New table** to create a new one to route and ingest the data.
    
8. Provide a **Data connection name** or keep the name provided, and then select **Next**. It can take a few minutes to pull data from the eventstream.
    
    ![A screenshot of the Get data screen for the KQL Database destination, with the Next button highlighted.](https://learn.microsoft.com/en-us/fabric/real-time-intelligence/event-streams/media/add-destination-kql-database/select-table.png)
    
9. On the **Inspect the data** screen, you can:
    
    - Select a **Format** to preview how the data is sent to your Eventhouse.
    - Select **Edit columns** to configure the columns for your data.
    - Select **Advanced** to select events to include or to choose mapping options.
    
    [![A screenshot showing the data formats and Advanced options on the Inspect the data screen.](https://learn.microsoft.com/en-us/fabric/real-time-intelligence/event-streams/media/add-destination-kql-database/select-format.png)](https://learn.microsoft.com/en-us/fabric/real-time-intelligence/event-streams/media/add-destination-kql-database/select-format.png#lightbox)
    
10. If you select **Edit columns**, on the **Edit columns** screen you can:
    
    - Select **Add column** to add a column.
    - Select **Source** columns to map.
    - Apply **Mapping transformation** to columns.
    - Change **Sample data** values.
    
    Then select **Apply**.
    
    [![A screenshot of the Edit columns screen.](https://learn.microsoft.com/en-us/fabric/real-time-intelligence/event-streams/media/add-destination-kql-database/edit-columns.png)](https://learn.microsoft.com/en-us/fabric/real-time-intelligence/event-streams/media/add-destination-kql-database/edit-columns.png#lightbox)
    
11. When you're finished configuring the data, select **Finish** on the **Inspect the data** screen.
    
12. On the **Summary** screen, review the details and status of your data ingestion, including the table with the schema you defined and the connection between the eventstream and the Eventhouse. Select **Close** to finalize the Eventhouse setup.
    
    [![A screenshot of the Summary screen with the Close button highlighted.](https://learn.microsoft.com/en-us/fabric/real-time-intelligence/event-streams/media/add-destination-kql-database/summary.png)](https://learn.microsoft.com/en-us/fabric/real-time-intelligence/event-streams/media/add-destination-kql-database/summary.png#lightbox)
    

You can now see the Eventhouse destination on the canvas in **Live view**.

[![A screenshot of the configured KQL Database destination in Live view.](https://learn.microsoft.com/en-us/fabric/real-time-intelligence/event-streams/media/add-destination-kql-database/live-view-finished.png)](https://learn.microsoft.com/en-us/fabric/real-time-intelligence/event-streams/media/add-destination-kql-database/live-view-finished.png#lightbox)

# Event processing before ingestion

The event processing before ingestion mode processes your event data before ingesting it into the Eventhouse. Use this mode if you apply operators such as filtering or aggregation to process the data before ingestion, or after a derived stream.

1. In **Edit mode** for your eventstream, hover over an operator or derived stream, select **+**, and then select **Eventhouse**.
    
    [![A screenshot of selecting the + symbol for the operator output and selecting KQL Database.](https://learn.microsoft.com/en-us/fabric/real-time-intelligence/event-streams/media/add-destination-kql-database/select-eventhouse.png)](https://learn.microsoft.com/en-us/fabric/real-time-intelligence/event-streams/media/add-destination-kql-database/select-eventhouse.png#lightbox)
    
2. On the **Eventhouse** screen, **Event processing before ingestion** should already be selected. Complete the rest of the information about your Eventhouse, and then select **Save**.
    
    ![A screenshot of the KQL Database configuration screen for Event processing before ingestion.](https://learn.microsoft.com/en-us/fabric/real-time-intelligence/event-streams/media/add-destination-kql-database/eventhouse-event-processing.png)
    
3. To implement the newly added Eventhouse destination, select **Publish**.
    
    [![A screenshot of the eventstream in Edit mode with the KQL Database destination added.](https://learn.microsoft.com/en-us/fabric/real-time-intelligence/event-streams/media/add-destination-kql-database/edit-mode-processed.png)](https://learn.microsoft.com/en-us/fabric/real-time-intelligence/event-streams/media/add-destination-kql-database/edit-mode-processed.png#lightbox)
    

Once you complete these steps, the eventstream with Eventhouse destination is available for visualization in **Live view**.

[![A screenshot of the configured KQL Database event processing flow in Live view.](https://learn.microsoft.com/en-us/fabric/real-time-intelligence/event-streams/media/add-destination-kql-database/live-view-processed-eventhouse.png)](https://learn.microsoft.com/en-us/fabric/real-time-intelligence/event-streams/media/add-destination-kql-database/live-view-processed-eventhouse.png#lightbox)