# MTA-GTFS-ADA-Subway-Stations
MTA/NYCT's stops.txt file was modified to include a column indicating if stations are ADA accessible.

Added two columnns:

Column 1: "ada_tc"
 "1" indicates stop_id's that are ADA accessible (i.e. street level or has an elevator)
 "0" indicates the stop is non-ADA accessible 
 
  The stop_id's tagged are the ones with an "N" or "S" at the end of their name. We did not assign the parent station with an accessibility indicator.

  In some cases (roughly 6 or 7 cases) a station will only be ADA accessible going one direction. For example, stop 109S (Dyckman St) is marked as being ADA compliant while 109N is not. This is because the northbound side of that station is not ADA accessible.
 
Column 2: "out_of_service_tc"
 "1" indicates stations that are long-term out of service, such as South Ferry on the 1 line or Brooklyn Bridge City Hall on the 456
 "0" means the station is operating

If the stop has a 1 in the out_of_service_tc column, it usually applies to both the "N" and "S" because it means the existing elevator(s) are currently undergoing construction or refurbishment, or the stop is offline completely, thus rendering what would otherwise have been an accessible station currently inaccessible.
