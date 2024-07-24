---
title: Welcome to Evidence
---

<Details title='How to edit this page'>

  This page can be found in your project at `/pages/index.md`. Make a change to the markdown file and save it to see the change take effect in your browser.
</Details>

<Dropdown name=species>
    <DropdownOption value=% valueLabel="All Species"/>
    <DropdownOption value=setosa/>
    <DropdownOption value=versicolor/>
    <DropdownOption value=virginica/>
</Dropdown>




```sql iris
SELECT * FROM Iris.iris
where species like '${inputs.species.value}'
```

<ScatterPlot
    data={iris}
    title="Iris"
    x=sepal_length
    y=sepal_width
    series=species
/>

## What's Next?
- [Connect your data sources](settings)
- Edit/add markdown files in the `pages` folder
- Deploy your project with [Evidence Cloud](https://evidence.dev/cloud)

## Get Support
- Message us on [Slack](https://slack.evidence.dev/)
- Read the [Docs](https://docs.evidence.dev/)
- Open an issue on [Github](https://github.com/evidence-dev/evidence)
