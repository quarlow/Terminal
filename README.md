# Terminal
Terminal Watchface

watchface.xml

<?xml version="1.0" encoding="utf-8" standalone="no"?>
<watchface device_name="Gear S2, Gear S3, Gear Sport, Galaxy Watch" height="360" name="watchface.xml" schema_version="1.5" screen_type="1" version="1.6.0" width="360">
    <root height="360" type="normal" width="360" x="0" y="0">
        <image action_type="image-set" height="360" id="Back" name="black.png" tap="double-tap" width="360" x="0" y="0">
            <condition source="battery">
                <section end="100" start="0"/>
            </condition>
            <image-set>
                <image>action/image/gray.png</image>
                <image>action/image/blue.png</image>
            </image-set>
        </image>
        <text alignment="16384" b="255" bitmap_font="false" custom_font="true" font_name="SourceCodePro-Medium" g="255" height="40" id="Prefix" locale="en_US" r="255" size="18" source="none" style="0" text=" " width="250" x="52" y="51"/>
        <text alignment="16384" b="255" bitmap_font="false" custom_font="true" font_name="SourceCodePro-Medium" g="255" height="40" id="cur_time" locale="en_US" r="255" size="24" source="none" style="0" text="user@watch:~ $ now" width="295" x="45" y="53"/>
        <text alignment="16384" b="170" bitmap_font="false" custom_font="true" font_name="SourceCodePro-Medium" g="170" height="40" id="TIME" locale="en_US" r="170" size="24" source="none" style="0" text="[TIME]" width="88" x="40" y="88"/>
        <text alignment="16384" b="170" bitmap_font="false" custom_font="true" font_name="SourceCodePro-Medium" g="170" height="40" id="DATE" locale="en_US" r="170" size="24" source="none" style="0" text="[DATE]" width="88" x="40" y="125"/>
        <digitalclock alignment="16384" b="170" bitmap_font="false" custom_font="true" font_name="SourceCodePro-Medium" g="170" height="35" id="Date Val" locale="en_US" r="0" size="24" style="0" text="E MMM dd yyyy" width="220" x="127" y="128"/>
        <text alignment="16384" b="170" bitmap_font="false" custom_font="true" font_name="SourceCodePro-Medium" g="170" height="40" id="BATT" locale="en_US" r="170" size="24" source="none" style="0" text="[BATT]" width="88" x="40" y="162"/>
        <text alignment="16384" b="170" bitmap_font="false" custom_font="true" font_name="SourceCodePro-Medium" g="170" height="40" id="STEP" locale="en_US" r="170" size="24" source="none" style="0" text="[STEP]" width="88" x="40" y="199"/>
        <text alignment="16384" b="0" bitmap_font="false" custom_font="true" font_name="SourceCodePro-Medium" g="170" height="32" id="Step Count 100" locale="en_US" postfix=" steps" r="0" size="24" source="pedometer.step" style="0" text="Text" width="221" x="127" y="203">
            <condition source="workout">
                <section end="100" start="100"/>
            </condition>
        </text>
        <text action_type="open-app" alignment="16384" b="170" bitmap_font="false" custom_font="true" font_name="SourceCodePro-Medium" g="0" height="32" id="Step Count" locale="en_US" postfix=" steps" r="170" size="24" source="pedometer.step" style="0" text="Text" width="221" x="127" y="203">
            <condition source="workout">
                <section end="99" start="0"/>
            </condition>
            <open-app preset="pedometer"/>
        </text>
        <text alignment="16384" b="170" bitmap_font="false" custom_font="true" font_name="SourceCodePro-Medium" g="170" height="40" id="L_HR" locale="en_US" r="170" size="24" source="none" style="0" text="[L_HR]" width="88" x="40" y="236"/>
        <text action_type="open-app" alignment="16384" b="51" bitmap_font="false" custom_font="true" font_name="SourceCodePro-Medium" g="51" height="32" id="Heart Rate" locale="en_US" postfix=" bpm" r="255" size="24" source="heartrate.recent" style="0" text="Text" width="220" x="128" y="240">
            <open-app preset="heartrate"/>
        </text>
        <text alignment="16384" b="255" bitmap_font="false" custom_font="true" font_name="SourceCodePro-Medium" g="255" height="40" id="Null" locale="en_US" r="255" size="24" source="none" style="0" text="user@watch:~ $ " width="295" x="44" y="268"/>
        <digitalclock alignment="16384" b="0" bitmap_font="false" custom_font="true" font_name="SourceCodePro-Medium" g="170" height="35" id="24H" locale="en_US" r="0" size="24" style="0" text="HH:mm:ss O" width="220" x="128" y="91">
            <condition source="hour12h24h">
                <section end="1" start="1"/>
            </condition>
        </digitalclock>
        <digitalclock alignment="16384" b="0" bitmap_font="false" custom_font="true" font_name="SourceCodePro-Medium" g="170" height="35" id="12H" locale="en_US" r="0" size="24" style="0" text="h:mm:ss a z" width="220" x="128" y="91">
            <condition source="hour12h24h">
                <section end="0" start="0"/>
            </condition>
        </digitalclock>
        <text alignment="16384" b="0" bitmap_font="false" custom_font="true" font_name="SourceCodePro-Medium" g="170" height="32" id="Batt Level 4" locale="en_US" r="0" size="24" source="battery.percent" style="0" text="Text" width="50" x="297" y="166">
            <condition source="battery">
                <section end="100" start="100"/>
            </condition>
        </text>
        <text alignment="16384" b="0" bitmap_font="false" custom_font="true" font_name="SourceCodePro-Medium" g="170" height="32" id="Batt Level 3" locale="en_US" postfix=" %" r="0" size="24" source="battery.percent" style="0" text="Text" width="62" x="295" y="166">
            <condition source="battery">
                <section end="99" start="30"/>
            </condition>
        </text>
        <text alignment="16384" b="0" bitmap_font="false" custom_font="true" font_name="SourceCodePro-Medium" g="170" height="32" id="Batt Level 2" locale="en_US" postfix=" %" r="255" size="24" source="battery.percent" style="0" text="Text" width="62" x="295" y="166">
            <condition source="battery">
                <section end="29" start="16"/>
            </condition>
        </text>
        <text alignment="16384" b="0" bitmap_font="false" custom_font="true" font_name="SourceCodePro-Medium" g="0" height="32" id="Batt Level 1" locale="en_US" postfix=" %" r="170" size="24" source="battery.percent" style="0" text="Text" width="62" x="295" y="166">
            <condition source="battery">
                <section end="15" start="0"/>
            </condition>
        </text>
        <text alignment="16384" b="0" bitmap_font="false" custom_font="true" font_name="SourceCodePro-Medium" g="170" height="32" id="Batt 10" locale="en_US" r="0" size="24" source="none" style="0" text="[##########]" width="171" x="124" y="166">
            <condition source="battery">
                <section end="100" start="95"/>
            </condition>
        </text>
        <text alignment="16384" b="0" bitmap_font="false" custom_font="true" font_name="SourceCodePro-Medium" g="170" height="32" id="Batt 9" locale="en_US" r="0" size="24" source="none" style="0" text="[#########.]" width="171" x="124" y="166">
            <condition source="battery">
                <section end="94" start="85"/>
            </condition>
        </text>
        <text alignment="16384" b="0" bitmap_font="false" custom_font="true" font_name="SourceCodePro-Medium" g="170" height="32" id="Batt 8" locale="en_US" r="0" size="24" source="none" style="0" text="[########..]" width="171" x="124" y="166">
            <condition source="battery">
                <section end="84" start="75"/>
            </condition>
        </text>
        <text alignment="16384" b="0" bitmap_font="false" custom_font="true" font_name="SourceCodePro-Medium" g="170" height="32" id="Batt 7" locale="en_US" r="0" size="24" source="none" style="0" text="[#######...]" width="171" x="124" y="166">
            <condition source="battery">
                <section end="74" start="65"/>
            </condition>
        </text>
        <text alignment="16384" b="0" bitmap_font="false" custom_font="true" font_name="SourceCodePro-Medium" g="170" height="32" id="Batt 6" locale="en_US" r="0" size="24" source="none" style="0" text="[######....]" width="171" x="124" y="166">
            <condition source="battery">
                <section end="64" start="55"/>
            </condition>
        </text>
        <text alignment="16384" b="0" bitmap_font="false" custom_font="true" font_name="SourceCodePro-Medium" g="170" height="32" id="Batt 5" locale="en_US" r="0" size="24" source="none" style="0" text="[#####.....]" width="171" x="124" y="166">
            <condition source="battery">
                <section end="54" start="45"/>
            </condition>
        </text>
        <text alignment="16384" b="0" bitmap_font="false" custom_font="true" font_name="SourceCodePro-Medium" g="170" height="32" id="Batt 4" locale="en_US" r="0" size="24" source="none" style="0" text="[####......]" width="171" x="124" y="166">
            <condition source="battery">
                <section end="44" start="35"/>
            </condition>
        </text>
        <text alignment="16384" b="0" bitmap_font="false" custom_font="true" font_name="SourceCodePro-Medium" g="170" height="32" id="Batt 3B" locale="en_US" r="0" size="24" source="none" style="0" text="[###.......]" width="171" x="124" y="166">
            <condition source="battery">
                <section end="34" start="30"/>
            </condition>
        </text>
        <text alignment="16384" b="0" bitmap_font="false" custom_font="true" font_name="SourceCodePro-Medium" g="170" height="32" id="Batt 3A" locale="en_US" r="255" size="24" source="none" style="0" text="[###.......]" width="171" x="124" y="166">
            <condition source="battery">
                <section end="29" start="25"/>
            </condition>
        </text>
        <text alignment="16384" b="0" bitmap_font="false" custom_font="true" font_name="SourceCodePro-Medium" g="170" height="32" id="Batt 2B" locale="en_US" r="255" size="24" source="none" style="0" text="[##........]" width="171" x="124" y="166">
            <condition source="battery">
                <section end="24" start="16"/>
            </condition>
        </text>
        <text alignment="16384" b="0" bitmap_font="false" custom_font="true" font_name="SourceCodePro-Medium" g="0" height="32" id="Batt 2A" locale="en_US" r="170" size="24" source="none" style="0" text="[##........]" width="171" x="124" y="166">
            <condition source="battery">
                <section end="15" start="15"/>
            </condition>
        </text>
        <text alignment="16384" b="0" bitmap_font="false" custom_font="true" font_name="SourceCodePro-Medium" g="0" height="32" id="Batt 1" locale="en_US" r="170" size="24" source="none" style="0" text="[#.........]" width="171" x="124" y="166">
            <condition source="battery">
                <section end="14" start="5"/>
            </condition>
        </text>
        <text alignment="16384" b="0" bitmap_font="false" custom_font="true" font_name="SourceCodePro-Medium" g="0" height="32" id="Batt 0" locale="en_US" r="170" size="24" source="none" style="0" text="[..........]" width="171" x="124" y="166">
            <condition source="battery">
                <section end="4" start="0"/>
            </condition>
        </text>
    </root>
    <root height="360" type="ambient" width="360" x="0" y="0">
        <digitalclock alignment="16777216" b="0" bitmap_font="false" custom_font="true" font_name="SourceCodePro-Medium" g="255" height="162" id="24H" locale="en_US" r="0" size="76" style="0" text="HH:mm" width="350" x="5" y="98">
            <condition source="hour12h24h">
                <section end="1" start="1"/>
            </condition>
        </digitalclock>
        <digitalclock alignment="16777216" b="0" bitmap_font="false" custom_font="true" font_name="SourceCodePro-Medium" g="255" height="162" id="12H" locale="en_US" r="0" size="76" style="0" text="h:mm" width="350" x="5" y="98">
            <condition source="hour12h24h">
                <section end="0" start="0"/>
            </condition>
        </digitalclock>
    </root>
    <root height="360" type="ambient-fullcolor" width="360" x="0" y="0">
        <image height="360" id="Back" name="black.png" width="360" x="0" y="0"/>
        <digitalclock alignment="16777216" b="0" bitmap_font="false" custom_font="true" font_name="SourceCodePro-Medium" g="170" height="162" id="24H" locale="en_US" r="0" size="76" style="0" text="HH:mm" width="345" x="10" y="98">
            <condition source="hour12h24h">
                <section end="1" start="1"/>
            </condition>
        </digitalclock>
        <digitalclock alignment="16777216" b="0" bitmap_font="false" custom_font="true" font_name="SourceCodePro-Medium" g="170" height="162" id="12H" locale="en_US" r="0" size="76" style="0" text="h:mm" width="345" x="10" y="98">
            <condition source="hour12h24h">
                <section end="0" start="0"/>
            </condition>
        </digitalclock>
    </root>
</watchface>
