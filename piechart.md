HighCharts.chart('<div name>', {
      chart: {
        plotBackgroundColor: null,
        plotBorderWidth: null,
        plotShadow: false,
        type: 'pie',
        height:150
      },
      title: {
        text: null
      },
      credits: {
        enabled: false
      },
      tooltip: {
         pointFormat: '{series.name}: <b>{point.percentage:.1f}%</b>'
      },
      plotOptions: {
        pie: {
          size: 104,
          allowPointSelect: true,
          cursor: 'pointer',
          "enableMouseTracking": true,
          "center": ["47%", "44%"],
          "connectorPadding": 3,
          "dataLabels": {
            "useHTML": true,
            "className": 'pieMainCatg',
            "style": {
              "width": '50px',
              "color": '#000',
              "text-decoration": 'none',
              'font-weight':'normal'
            },
            "maxStaggerLines": 2,
            "crop": false,
            "softConnector": false,
            "align": 'right',
            "overflow": "justify",
            "enabled": true,
            "distance": 5,
            "format": "<div class='tipHldr'><div class='tipName'>{point.name}</div></div>"
          }

        }
      },

      series: [{
        name: '<data name>',
        data: [
          { name: '<data name 1>', y: 25 },
          { name: '<data name 2>', y: 25 },
          { name: '<data name 3>', y: 25 },
          { name: '<data name 4>', y: 25 }
        ]
      }]
    });
    
    
    #demo https://jsfiddle.net/jophine/cuf07pw8/
