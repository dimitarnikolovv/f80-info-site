<script>
    import 'charts.css';
</script>

<div id="line-chart-wrap">
    <table
        id="line-chart"
        class="charts-css show-heading line multiple show-labels show-data-on-hover show-10-secondary-axes show-primary-axis"
    >
        <caption> Car Accidents </caption>

        <tbody>
            <tr>
                <th scope="row"> Label </th>
                <td style="--start: 0.0; --size: 0.2">
                    <span class="data"> <strong>.</strong> </span>
                    <span class="tooltip"> Data: 30 <br /> More info... </span>
                </td>
                <td style="--start: 0.0; --size: 0.1; --color: lightgreen">
                    <span class="data"> <strong>.</strong> </span>
                    <span class="tooltip"> Data: 30 <br /> More info... </span>
                </td>
            </tr>
            <tr>
                <th scope="row"> Label </th>
                <td style="--start: 0.2; --size: 0.3">
                    <span class="data"> <strong>.</strong> </span>
                    <span class="tooltip"> Data: 30 <br /> More info... </span>
                </td>
                <td style="--start: 0.1; --size: 0.3; --color: lightgreen">
                    <span class="data"> <strong>.</strong> </span>
                    <span class="tooltip"> Data: 30 <br /> More info... </span>
                </td>
            </tr>
            <tr>
                <th scope="row"> Label </th>
                <td style="--start: 0.3; --size: 0.5">
                    <span class="data"> <strong>.</strong> </span>
                    <span class="tooltip"> Data: 30 <br /> More info... </span>
                </td>
                <td style="--start: 0.3; --size: 0.2; --color: lightgreen">
                    <span class="data"> <strong>.</strong> </span>
                    <span class="tooltip"> Data: 30 <br /> More info... </span>
                </td>
            </tr>
            <tr>
                <th scope="row"> Label </th>
                <td style="--start: 0.5; --size: 0.5">
                    <span class="data"> <strong>.</strong></span>
                    <span class="tooltip"> Data: 30 <br /> More info... </span>
                </td>
                <td style="--start: 0.2; --size: 0.4; --color: lightgreen">
                    <span class="data"> <strong>.</strong> </span>
                    <span class="tooltip"> Data: 30 <br /> More info... </span>
                </td>
            </tr>
            <tr>
                <th scope="row"> Label </th>
                <td style="--start: 0.5; --size: 0.4">
                    <span class="data"> <strong>.</strong> </span>
                    <span class="tooltip">Data: 30 <br /> More info...</span>
                </td>
                <td style="--start: 0.4; --size: 0.5; --color: lightgreen">
                    <span class="data"> <strong>.</strong> </span>
                    <span class="tooltip"> Data: 30 <br /> More info... </span>
                </td>
            </tr>
            <tr>
                <th scope="row"> Label </th>
                <td style="--start: 0.4; --size: 0.4">
                    <span class="data"> <strong>.</strong> </span>
                    <span class="tooltip"> Data: 30 <br /> More info... </span>
                </td>
                <td style="--start: 0.5; --size: 0.4; --color: lightgreen">
                    <span class="data"> <strong>.</strong> </span>
                    <span class="tooltip"> Data: 30 <br /> More info... </span>
                </td>
            </tr>
            <tr>
                <th scope="row"> Label </th>
                <td style="--start: 0.4; --size: 0.6">
                    <span class="data"> <strong>.</strong> </span>
                    <span class="tooltip"> Data: 30 <br /> More info... </span>
                </td>
                <td style="--start: 0.4; --size: 0.4; --color: lightgreen">
                    <span class="data"> <strong>.</strong> </span>
                    <span class="tooltip"> Data: 30 <br /> More info... </span>
                </td>
            </tr>
            <tr>
                <th scope="row"> Label </th>
                <td style="--start: 0.6; --size: 0.7">
                    <span class="data"> <strong>.</strong> </span>
                    <span class="tooltip"> Data: 30 <br /> More info... </span>
                </td>
                <td style="--start: 0.4; --size: 0.6; --color: lightgreen">
                    <span class="data"> <strong>.</strong> </span>
                    <span class="tooltip"> Data: 30 <br /> More info... </span>
                </td>
            </tr>
        </tbody>
    </table>
    <ul id="line-chart-legend" class="charts-css legend legend-line">
        <li class="--color: lightred">Label 1</li>
        <li class="--color: lightgreen">Label 2</li>
        <li>Label 3</li>
    </ul>
</div>

<style lang="scss">
    #line-chart-wrap {
        display: flex;
        flex-direction: column;
        justify-content: center;
        gap: 2rem;
        height: 60vh;
    }
    #line-chart-legend {
        flex-direction: row;
        justify-content: space-between;
        height: 20%;
        width: 80%;
        border: none;

        @media only screen and (max-width: 620px) {
            width: 100%;
        }

        @media only screen and (max-width: 400px) {
            flex-direction: column;
            justify-content: center;
            align-items: center;
        }

        li:nth-child(1) {
            &::before {
                background-color: rgba(240, 50, 50, 0.75);
            }
        }

        li:nth-child(2) {
            &::before {
                background-color: lightgreen;
            }
        }
    }
    #line-chart {
        width: 80%;
        margin: 0 auto;

        @media only screen and (max-width: 620px) {
            height: 60%;
            width: 100%;
        }
    }
</style>
