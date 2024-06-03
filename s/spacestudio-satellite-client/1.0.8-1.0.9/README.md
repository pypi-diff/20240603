# Comparing `tmp/spacestudio-satellite-client-1.0.8.tar.gz` & `tmp/spacestudio-satellite-client-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spacestudio-satellite-client-1.0.8.tar", last modified: Thu Feb 29 13:43:59 2024, max compression
+gzip compressed data, was "spacestudio-satellite-client-1.0.9.tar", last modified: Thu Feb 29 14:26:34 2024, max compression
```

## Comparing `spacestudio-satellite-client-1.0.8.tar` & `spacestudio-satellite-client-1.0.9.tar`

### file list

```diff
@@ -1,167 +1,167 @@
-drwxrwxrwx   0        0        0        0 2024-02-29 13:43:59.560876 spacestudio-satellite-client-1.0.8/
--rw-rw-rw-   0        0        0      570 2024-02-29 13:43:59.559876 spacestudio-satellite-client-1.0.8/PKG-INFO
--rw-rw-rw-   0        0        0    11988 2024-02-29 13:43:20.000000 spacestudio-satellite-client-1.0.8/README.md
--rw-rw-rw-   0        0        0     2020 2024-02-29 13:43:20.000000 spacestudio-satellite-client-1.0.8/pyproject.toml
--rw-rw-rw-   0        0        0       76 2024-02-29 13:43:59.562880 spacestudio-satellite-client-1.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1414 2024-02-29 13:43:20.000000 spacestudio-satellite-client-1.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2024-02-29 13:43:59.397746 spacestudio-satellite-client-1.0.8/spacestudio_satellite_client/
--rw-rw-rw-   0        0        0     7406 2024-02-29 13:43:20.000000 spacestudio-satellite-client-1.0.8/spacestudio_satellite_client/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-29 13:43:59.430875 spacestudio-satellite-client-1.0.8/spacestudio_satellite_client/api/
--rw-rw-rw-   0        0        0      744 2024-02-29 13:43:20.000000 spacestudio-satellite-client-1.0.8/spacestudio_satellite_client/api/__init__.py
--rw-rw-rw-   0        0        0    30710 2024-02-29 13:43:20.000000 spacestudio-satellite-client-1.0.8/spacestudio_satellite_client/api/announcement_api.py
--rw-rw-rw-   0        0        0    19800 2024-02-29 13:43:20.000000 spacestudio-satellite-client-1.0.8/spacestudio_satellite_client/api/computations_api.py
--rw-rw-rw-   0        0        0    21182 2024-02-29 13:43:20.000000 spacestudio-satellite-client-1.0.8/spacestudio_satellite_client/api/notification_api.py
--rw-rw-rw-   0        0        0    51641 2024-02-29 13:43:20.000000 spacestudio-satellite-client-1.0.8/spacestudio_satellite_client/api/orbits_api.py
--rw-rw-rw-   0        0        0    52103 2024-02-29 13:43:20.000000 spacestudio-satellite-client-1.0.8/spacestudio_satellite_client/api/platforms_api.py
--rw-rw-rw-   0        0        0    53440 2024-02-29 13:43:20.000000 spacestudio-satellite-client-1.0.8/spacestudio_satellite_client/api/propulsion_systems_api.py
--rw-rw-rw-   0        0        0    72103 2024-02-29 13:43:20.000000 spacestudio-satellite-client-1.0.8/spacestudio_satellite_client/api/scenarios_api.py
--rw-rw-rw-   0        0        0    53736 2024-02-29 13:43:20.000000 spacestudio-satellite-client-1.0.8/spacestudio_satellite_client/api/spacecraft_geometries_api.py
--rw-rw-rw-   0        0        0    77009 2024-02-29 13:43:20.000000 spacestudio-satellite-client-1.0.8/spacestudio_satellite_client/api/studies_api.py
--rw-rw-rw-   0        0        0    25897 2024-02-29 13:43:20.000000 spacestudio-satellite-client-1.0.8/spacestudio_satellite_client/api_client.py
--rw-rw-rw-   0        0        0      652 2024-02-29 13:43:20.000000 spacestudio-satellite-client-1.0.8/spacestudio_satellite_client/api_response.py
--rw-rw-rw-   0        0        0    14838 2024-02-29 13:43:20.000000 spacestudio-satellite-client-1.0.8/spacestudio_satellite_client/configuration.py
--rw-rw-rw-   0        0        0     5994 2024-02-29 13:43:20.000000 spacestudio-satellite-client-1.0.8/spacestudio_satellite_client/exceptions.py
-drwxrwxrwx   0        0        0        0 2024-02-29 13:43:59.489875 spacestudio-satellite-client-1.0.8/spacestudio_satellite_client/models/
--rw-rw-rw-   0        0        0     6040 2024-02-29 13:43:20.000000 spacestudio-satellite-client-1.0.8/spacestudio_satellite_client/models/__init__.py
--rw-rw-rw-   0        0        0     5157 2024-02-29 13:43:19.000000 spacestudio-satellite-client-1.0.8/spacestudio_satellite_client/models/advanced_orbit_parameters.py
--rw-rw-rw-   0        0        0     3440 2024-02-29 13:43:19.000000 spacestudio-satellite-client-1.0.8/spacestudio_satellite_client/models/analytical_study_parameters.py
--rw-rw-rw-   0        0        0     3302 2024-02-29 13:43:19.000000 spacestudio-satellite-client-1.0.8/spacestudio_satellite_client/models/announcement.py
--rw-rw-rw-   0        0        0     2960 2024-02-29 13:43:19.000000 spacestudio-satellite-client-1.0.8/spacestudio_satellite_client/models/baseline_configuration.py
--rw-rw-rw-   0        0        0     2851 2024-02-29 13:43:19.000000 spacestudio-satellite-client-1.0.8/spacestudio_satellite_client/models/circular_altitude_orbit_parameters.py
--rw-rw-rw-   0        0        0     3097 2024-02-29 13:43:19.000000 spacestudio-satellite-client-1.0.8/spacestudio_satellite_client/models/circular_ground_track_repeated_orbit_parameters.py
--rw-rw-rw-   0        0        0     4574 2024-02-29 13:43:19.000000 spacestudio-satellite-client-1.0.8/spacestudio_satellite_client/models/comparison_item.py
--rw-rw-rw-   0        0        0     4578 2024-02-29 13:43:19.000000 spacestudio-satellite-client-1.0.8/spacestudio_satellite_client/models/comparison_item1.py
--rw-rw-rw-   0        0        0     4516 2024-02-29 13:43:19.000000 spacestudio-satellite-client-1.0.8/spacestudio_satellite_client/models/computation.py
--rw-rw-rw-   0        0        0      794 2024-02-29 13:43:19.000000 spacestudio-satellite-client-1.0.8/spacestudio_satellite_client/models/computation_mode.py
--rw-rw-rw-   0        0        0     3753 2024-02-29 13:43:35.000000 spacestudio-satellite-client-1.0.8/spacestudio_satellite_client/models/computation_outputs.py
--rw-rw-rw-   0        0        0      890 2024-02-29 13:43:19.000000 spacestudio-satellite-client-1.0.8/spacestudio_satellite_client/models/computation_status.py
--rw-rw-rw-   0        0        0      794 2024-02-29 13:43:19.000000 spacestudio-satellite-client-1.0.8/spacestudio_satellite_client/models/computation_type.py
--rw-rw-rw-   0        0        0     2736 2024-02-29 13:43:19.000000 spacestudio-satellite-client-1.0.8/spacestudio_satellite_client/models/context_outputs.py
--rw-rw-rw-   0        0        0     2476 2024-02-29 13:43:19.000000 spacestudio-satellite-client-1.0.8/spacestudio_satellite_client/models/deorbitation.py
--rw-rw-rw-   0        0        0     4590 2024-02-29 13:43:19.000000 spacestudio-satellite-client-1.0.8/spacestudio_satellite_client/models/display_configuration.py
--rw-rw-rw-   0        0        0     3684 2024-02-29 13:43:19.000000 spacestudio-satellite-client-1.0.8/spacestudio_satellite_client/models/display_configuration_comparison_overview.py
--rw-rw-rw-   0        0        0     2885 2024-02-29 13:43:19.000000 spacestudio-satellite-client-1.0.8/spacestudio_satellite_client/models/drag_perturbation.py
--rw-rw-rw-   0        0        0     2621 2024-02-29 13:43:19.000000 spacestudio-satellite-client-1.0.8/spacestudio_satellite_client/models/duplicate_scenario_request.py
--rw-rw-rw-   0        0        0      818 2024-02-29 13:43:19.000000 spacestudio-satellite-client-1.0.8/spacestudio_satellite_client/models/earth_potential_configuration.py
--rw-rw-rw-   0        0        0     3545 2024-02-29 13:43:19.000000 spacestudio-satellite-client-1.0.8/spacestudio_satellite_client/models/earth_potential_perturbation.py
--rw-rw-rw-   0        0        0     3153 2024-02-29 13:43:19.000000 spacestudio-satellite-client-1.0.8/spacestudio_satellite_client/models/elliptical_ground_track_repeated_eccentricity_orbit_parameters.py
--rw-rw-rw-   0        0        0     3200 2024-02-29 13:43:19.000000 spacestudio-satellite-client-1.0.8/spacestudio_satellite_client/models/elliptical_perigee_alt_apogee_alt_orbit_parameters.py
--rw-rw-rw-   0        0        0     2977 2024-02-29 13:43:19.000000 spacestudio-satellite-client-1.0.8/spacestudio_satellite_client/models/elliptical_perigee_alt_eccentricity_orbit_parameters.py
--rw-rw-rw-   0        0        0     2640 2024-02-29 13:43:19.000000 spacestudio-satellite-client-1.0.8/spacestudio_satellite_client/models/elliptical_sma_eccentricity_orbit_parameters.py
--rw-rw-rw-   0        0        0     3457 2024-02-29 13:43:19.000000 spacestudio-satellite-client-1.0.8/spacestudio_satellite_client/models/leo_station_keeping.py
--rw-rw-rw-   0        0        0     4271 2024-02-29 13:43:37.000000 spacestudio-satellite-client-1.0.8/spacestudio_satellite_client/models/maneuver.py
--rw-rw-rw-   0        0        0     4569 2024-02-29 13:43:19.000000 spacestudio-satellite-client-1.0.8/spacestudio_satellite_client/models/maneuver_timeline_slot.py
--rw-rw-rw-   0        0        0     6661 2024-02-29 13:43:20.000000 spacestudio-satellite-client-1.0.8/spacestudio_satellite_client/models/maneuvering_strategy.py
--rw-rw-rw-   0        0        0     3805 2024-02-29 13:43:20.000000 spacestudio-satellite-client-1.0.8/spacestudio_satellite_client/models/notification.py
--rw-rw-rw-   0        0        0     2723 2024-02-29 13:43:20.000000 spacestudio-satellite-client-1.0.8/spacestudio_satellite_client/models/notification_content.py
--rw-rw-rw-   0        0        0     2815 2024-02-29 13:43:20.000000 spacestudio-satellite-client-1.0.8/spacestudio_satellite_client/models/numerical_ephemeris.py
--rw-rw-rw-   0        0        0     5113 2024-02-29 13:43:20.000000 spacestudio-satellite-client-1.0.8/spacestudio_satellite_client/models/numerical_outputs_configuration.py
--rw-rw-rw-   0        0        0     5429 2024-02-29 13:43:20.000000 spacestudio-satellite-client-1.0.8/spacestudio_satellite_client/models/numerical_study_parameters.py
--rw-rw-rw-   0        0        0     4704 2024-02-29 13:43:20.000000 spacestudio-satellite-client-1.0.8/spacestudio_satellite_client/models/orbit.py
--rw-rw-rw-   0        0        0     4893 2024-02-29 13:43:41.000000 spacestudio-satellite-client-1.0.8/spacestudio_satellite_client/models/orbit_parameters.py
--rw-rw-rw-   0        0        0     3621 2024-02-29 13:43:20.000000 spacestudio-satellite-client-1.0.8/spacestudio_satellite_client/models/orbit_phasing.py
--rw-rw-rw-   0        0        0     2734 2024-02-29 13:43:20.000000 spacestudio-satellite-client-1.0.8/spacestudio_satellite_client/models/orbit_propagation.py
--rw-rw-rw-   0        0        0     2969 2024-02-29 13:43:20.000000 spacestudio-satellite-client-1.0.8/spacestudio_satellite_client/models/orbit_timeline_slot.py
--rw-rw-rw-   0        0        0     2488 2024-02-29 13:43:20.000000 spacestudio-satellite-client-1.0.8/spacestudio_satellite_client/models/orbital_transfer.py
--rw-rw-rw-   0        0        0     2802 2024-02-29 13:43:20.000000 spacestudio-satellite-client-1.0.8/spacestudio_satellite_client/models/payload.py
--rw-rw-rw-   0        0        0     3783 2024-02-29 13:43:43.000000 spacestudio-satellite-client-1.0.8/spacestudio_satellite_client/models/perturbation.py
--rw-rw-rw-   0        0        0      843 2024-02-29 13:43:20.000000 spacestudio-satellite-client-1.0.8/spacestudio_satellite_client/models/perturbation_type.py
--rw-rw-rw-   0        0        0     4464 2024-02-29 13:43:20.000000 spacestudio-satellite-client-1.0.8/spacestudio_satellite_client/models/platform.py
--rw-rw-rw-   0        0        0     3510 2024-02-29 13:43:20.000000 spacestudio-satellite-client-1.0.8/spacestudio_satellite_client/models/plot.py
--rw-rw-rw-   0        0        0     6472 2024-02-29 13:43:20.000000 spacestudio-satellite-client-1.0.8/spacestudio_satellite_client/models/propulsion_system.py
--rw-rw-rw-   0        0        0     5454 2024-02-29 13:43:20.000000 spacestudio-satellite-client-1.0.8/spacestudio_satellite_client/models/raan_phasing.py
--rw-rw-rw-   0        0        0     3731 2024-02-29 13:43:20.000000 spacestudio-satellite-client-1.0.8/spacestudio_satellite_client/models/scenario.py
--rw-rw-rw-   0        0        0     8722 2024-02-29 13:43:20.000000 spacestudio-satellite-client-1.0.8/spacestudio_satellite_client/models/scenario_baseline.py
--rw-rw-rw-   0        0        0     3360 2024-02-29 13:43:20.000000 spacestudio-satellite-client-1.0.8/spacestudio_satellite_client/models/simulation_configuration.py
--rw-rw-rw-   0        0        0     6152 2024-02-29 13:43:20.000000 spacestudio-satellite-client-1.0.8/spacestudio_satellite_client/models/single_satellite_analytical_computation_outputs.py
--rw-rw-rw-   0        0        0     5728 2024-02-29 13:43:20.000000 spacestudio-satellite-client-1.0.8/spacestudio_satellite_client/models/single_satellite_numerical_computation_outputs.py
--rw-rw-rw-   0        0        0     2659 2024-02-29 13:43:20.000000 spacestudio-satellite-client-1.0.8/spacestudio_satellite_client/models/solar_radiation_pressure_perturbation.py
--rw-rw-rw-   0        0        0    15511 2024-02-29 13:43:20.000000 spacestudio-satellite-client-1.0.8/spacestudio_satellite_client/models/spacecraft_geometry.py
--rw-rw-rw-   0        0        0     6204 2024-02-29 13:43:20.000000 spacestudio-satellite-client-1.0.8/spacestudio_satellite_client/models/study.py
--rw-rw-rw-   0        0        0     3966 2024-02-29 13:43:20.000000 spacestudio-satellite-client-1.0.8/spacestudio_satellite_client/models/study_computation.py
--rw-rw-rw-   0        0        0     7407 2024-02-29 13:43:20.000000 spacestudio-satellite-client-1.0.8/spacestudio_satellite_client/models/study_inputs.py
--rw-rw-rw-   0        0        0     4452 2024-02-29 13:43:45.000000 spacestudio-satellite-client-1.0.8/spacestudio_satellite_client/models/study_parameters.py
--rw-rw-rw-   0        0        0     3171 2024-02-29 13:43:20.000000 spacestudio-satellite-client-1.0.8/spacestudio_satellite_client/models/tab.py
--rw-rw-rw-   0        0        0     2607 2024-02-29 13:43:20.000000 spacestudio-satellite-client-1.0.8/spacestudio_satellite_client/models/third_body_perturbation.py
--rw-rw-rw-   0        0        0     1217 2024-02-29 13:43:20.000000 spacestudio-satellite-client-1.0.8/spacestudio_satellite_client/models/thrust_arcs_position.py
--rw-rw-rw-   0        0        0     4450 2024-02-29 13:43:46.000000 spacestudio-satellite-client-1.0.8/spacestudio_satellite_client/models/timeline_slot.py
--rw-rw-rw-   0        0        0        0 2024-02-29 13:43:20.000000 spacestudio-satellite-client-1.0.8/spacestudio_satellite_client/py.typed
--rw-rw-rw-   0        0        0     9268 2024-02-29 13:43:20.000000 spacestudio-satellite-client-1.0.8/spacestudio_satellite_client/rest.py
-drwxrwxrwx   0        0        0        0 2024-02-29 13:43:59.559876 spacestudio-satellite-client-1.0.8/spacestudio_satellite_client.egg-info/
--rw-rw-rw-   0        0        0      570 2024-02-29 13:43:59.000000 spacestudio-satellite-client-1.0.8/spacestudio_satellite_client.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     7423 2024-02-29 13:43:59.000000 spacestudio-satellite-client-1.0.8/spacestudio_satellite_client.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-29 13:43:59.000000 spacestudio-satellite-client-1.0.8/spacestudio_satellite_client.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       76 2024-02-29 13:43:59.000000 spacestudio-satellite-client-1.0.8/spacestudio_satellite_client.egg-info/requires.txt
--rw-rw-rw-   0        0        0       29 2024-02-29 13:43:59.000000 spacestudio-satellite-client-1.0.8/spacestudio_satellite_client.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-02-29 13:43:59.557878 spacestudio-satellite-client-1.0.8/test/
--rw-rw-rw-   0        0        0     1798 2024-02-29 13:16:03.000000 spacestudio-satellite-client-1.0.8/test/test_advanced_orbit_parameters.py
--rw-rw-rw-   0        0        0     1522 2024-02-29 13:16:03.000000 spacestudio-satellite-client-1.0.8/test/test_analytical_study_parameters.py
--rw-rw-rw-   0        0        0     1692 2024-02-29 13:16:03.000000 spacestudio-satellite-client-1.0.8/test/test_announcement.py
--rw-rw-rw-   0        0        0     1113 2024-02-29 13:16:03.000000 spacestudio-satellite-client-1.0.8/test/test_announcement_api.py
--rw-rw-rw-   0        0        0     1860 2024-02-29 13:16:03.000000 spacestudio-satellite-client-1.0.8/test/test_baseline_configuration.py
--rw-rw-rw-   0        0        0     1628 2024-02-29 13:16:03.000000 spacestudio-satellite-client-1.0.8/test/test_circular_altitude_orbit_parameters.py
--rw-rw-rw-   0        0        0     1809 2024-02-29 13:16:03.000000 spacestudio-satellite-client-1.0.8/test/test_circular_ground_track_repeated_orbit_parameters.py
--rw-rw-rw-   0        0        0     1812 2024-02-29 13:16:03.000000 spacestudio-satellite-client-1.0.8/test/test_comparison_item.py
--rw-rw-rw-   0        0        0     1824 2024-02-29 13:16:03.000000 spacestudio-satellite-client-1.0.8/test/test_comparison_item1.py
--rw-rw-rw-   0        0        0     2413 2024-02-29 13:16:03.000000 spacestudio-satellite-client-1.0.8/test/test_computation.py
--rw-rw-rw-   0        0        0      754 2024-02-29 13:16:03.000000 spacestudio-satellite-client-1.0.8/test/test_computation_mode.py
--rw-rw-rw-   0        0        0     1473 2024-02-29 13:16:03.000000 spacestudio-satellite-client-1.0.8/test/test_computation_outputs.py
--rw-rw-rw-   0        0        0      768 2024-02-29 13:16:03.000000 spacestudio-satellite-client-1.0.8/test/test_computation_status.py
--rw-rw-rw-   0        0        0      754 2024-02-29 13:16:03.000000 spacestudio-satellite-client-1.0.8/test/test_computation_type.py
--rw-rw-rw-   0        0        0      992 2024-02-29 13:16:03.000000 spacestudio-satellite-client-1.0.8/test/test_computations_api.py
--rw-rw-rw-   0        0        0     1436 2024-02-29 13:16:03.000000 spacestudio-satellite-client-1.0.8/test/test_context_outputs.py
--rw-rw-rw-   0        0        0     1364 2024-02-29 13:16:03.000000 spacestudio-satellite-client-1.0.8/test/test_deorbitation.py
--rw-rw-rw-   0        0        0     3991 2024-02-29 13:16:03.000000 spacestudio-satellite-client-1.0.8/test/test_display_configuration.py
--rw-rw-rw-   0        0        0     2186 2024-02-29 13:16:03.000000 spacestudio-satellite-client-1.0.8/test/test_display_configuration_comparison_overview.py
--rw-rw-rw-   0        0        0     1455 2024-02-29 13:16:03.000000 spacestudio-satellite-client-1.0.8/test/test_drag_perturbation.py
--rw-rw-rw-   0        0        0     1558 2024-02-29 13:16:03.000000 spacestudio-satellite-client-1.0.8/test/test_duplicate_scenario_request.py
--rw-rw-rw-   0        0        0      839 2024-02-29 13:16:03.000000 spacestudio-satellite-client-1.0.8/test/test_earth_potential_configuration.py
--rw-rw-rw-   0        0        0     1694 2024-02-29 13:16:03.000000 spacestudio-satellite-client-1.0.8/test/test_earth_potential_perturbation.py
--rw-rw-rw-   0        0        0     1978 2024-02-29 13:16:03.000000 spacestudio-satellite-client-1.0.8/test/test_elliptical_ground_track_repeated_eccentricity_orbit_parameters.py
--rw-rw-rw-   0        0        0     1836 2024-02-29 13:16:03.000000 spacestudio-satellite-client-1.0.8/test/test_elliptical_perigee_alt_apogee_alt_orbit_parameters.py
--rw-rw-rw-   0        0        0     1830 2024-02-29 13:16:03.000000 spacestudio-satellite-client-1.0.8/test/test_elliptical_perigee_alt_eccentricity_orbit_parameters.py
--rw-rw-rw-   0        0        0     1704 2024-02-29 13:16:03.000000 spacestudio-satellite-client-1.0.8/test/test_elliptical_sma_eccentricity_orbit_parameters.py
--rw-rw-rw-   0        0        0     1590 2024-02-29 13:16:03.000000 spacestudio-satellite-client-1.0.8/test/test_leo_station_keeping.py
--rw-rw-rw-   0        0        0     1358 2024-02-29 13:16:03.000000 spacestudio-satellite-client-1.0.8/test/test_maneuver.py
--rw-rw-rw-   0        0        0     4709 2024-02-29 13:16:03.000000 spacestudio-satellite-client-1.0.8/test/test_maneuver_timeline_slot.py
--rw-rw-rw-   0        0        0     2176 2024-02-29 13:16:03.000000 spacestudio-satellite-client-1.0.8/test/test_maneuvering_strategy.py
--rw-rw-rw-   0        0        0     1990 2024-02-29 13:16:03.000000 spacestudio-satellite-client-1.0.8/test/test_notification.py
--rw-rw-rw-   0        0        0      977 2024-02-29 13:16:03.000000 spacestudio-satellite-client-1.0.8/test/test_notification_api.py
--rw-rw-rw-   0        0        0     1536 2024-02-29 13:16:03.000000 spacestudio-satellite-client-1.0.8/test/test_notification_content.py
--rw-rw-rw-   0        0        0     1660 2024-02-29 13:16:03.000000 spacestudio-satellite-client-1.0.8/test/test_numerical_ephemeris.py
--rw-rw-rw-   0        0        0     1945 2024-02-29 13:16:03.000000 spacestudio-satellite-client-1.0.8/test/test_numerical_outputs_configuration.py
--rw-rw-rw-   0        0        0     3236 2024-02-29 13:16:03.000000 spacestudio-satellite-client-1.0.8/test/test_numerical_study_parameters.py
--rw-rw-rw-   0        0        0     2091 2024-02-29 13:16:03.000000 spacestudio-satellite-client-1.0.8/test/test_orbit.py
--rw-rw-rw-   0        0        0     1455 2024-02-29 13:16:03.000000 spacestudio-satellite-client-1.0.8/test/test_orbit_parameters.py
--rw-rw-rw-   0        0        0     1563 2024-02-29 13:16:03.000000 spacestudio-satellite-client-1.0.8/test/test_orbit_phasing.py
--rw-rw-rw-   0        0        0     1446 2024-02-29 13:16:03.000000 spacestudio-satellite-client-1.0.8/test/test_orbit_propagation.py
--rw-rw-rw-   0        0        0     2394 2024-02-29 13:16:03.000000 spacestudio-satellite-client-1.0.8/test/test_orbit_timeline_slot.py
--rw-rw-rw-   0        0        0     1401 2024-02-29 13:16:03.000000 spacestudio-satellite-client-1.0.8/test/test_orbital_transfer.py
--rw-rw-rw-   0        0        0     1284 2024-02-29 13:16:03.000000 spacestudio-satellite-client-1.0.8/test/test_orbits_api.py
--rw-rw-rw-   0        0        0     1383 2024-02-29 13:16:03.000000 spacestudio-satellite-client-1.0.8/test/test_payload.py
--rw-rw-rw-   0        0        0     1394 2024-02-29 13:16:03.000000 spacestudio-satellite-client-1.0.8/test/test_perturbation.py
--rw-rw-rw-   0        0        0      761 2024-02-29 13:16:03.000000 spacestudio-satellite-client-1.0.8/test/test_perturbation_type.py
--rw-rw-rw-   0        0        0     1692 2024-02-29 13:16:03.000000 spacestudio-satellite-client-1.0.8/test/test_platform.py
--rw-rw-rw-   0        0        0     1344 2024-02-29 13:16:03.000000 spacestudio-satellite-client-1.0.8/test/test_platforms_api.py
--rw-rw-rw-   0        0        0     1477 2024-02-29 13:16:03.000000 spacestudio-satellite-client-1.0.8/test/test_plot.py
--rw-rw-rw-   0        0        0     2018 2024-02-29 13:16:03.000000 spacestudio-satellite-client-1.0.8/test/test_propulsion_system.py
--rw-rw-rw-   0        0        0     1515 2024-02-29 13:16:03.000000 spacestudio-satellite-client-1.0.8/test/test_propulsion_systems_api.py
--rw-rw-rw-   0        0        0     1891 2024-02-29 13:16:03.000000 spacestudio-satellite-client-1.0.8/test/test_raan_phasing.py
--rw-rw-rw-   0        0        0     6570 2024-02-29 13:16:03.000000 spacestudio-satellite-client-1.0.8/test/test_scenario.py
--rw-rw-rw-   0        0        0     5853 2024-02-29 13:16:03.000000 spacestudio-satellite-client-1.0.8/test/test_scenario_baseline.py
--rw-rw-rw-   0        0        0     1611 2024-02-29 13:16:03.000000 spacestudio-satellite-client-1.0.8/test/test_scenarios_api.py
--rw-rw-rw-   0        0        0     1597 2024-02-29 13:16:03.000000 spacestudio-satellite-client-1.0.8/test/test_simulation_configuration.py
--rw-rw-rw-   0        0        0     2431 2024-02-29 13:16:03.000000 spacestudio-satellite-client-1.0.8/test/test_single_satellite_analytical_computation_outputs.py
--rw-rw-rw-   0        0        0     2606 2024-02-29 13:16:03.000000 spacestudio-satellite-client-1.0.8/test/test_single_satellite_numerical_computation_outputs.py
--rw-rw-rw-   0        0        0     1631 2024-02-29 13:16:03.000000 spacestudio-satellite-client-1.0.8/test/test_solar_radiation_pressure_perturbation.py
--rw-rw-rw-   0        0        0     1566 2024-02-29 13:16:03.000000 spacestudio-satellite-client-1.0.8/test/test_spacecraft_geometries_api.py
--rw-rw-rw-   0        0        0     3509 2024-02-29 13:16:03.000000 spacestudio-satellite-client-1.0.8/test/test_spacecraft_geometry.py
--rw-rw-rw-   0        0        0     1614 2024-02-29 13:16:04.000000 spacestudio-satellite-client-1.0.8/test/test_studies_api.py
--rw-rw-rw-   0        0        0    11380 2024-02-29 13:16:04.000000 spacestudio-satellite-client-1.0.8/test/test_study.py
--rw-rw-rw-   0        0        0     3974 2024-02-29 13:16:04.000000 spacestudio-satellite-client-1.0.8/test/test_study_computation.py
--rw-rw-rw-   0        0        0     7220 2024-02-29 13:16:04.000000 spacestudio-satellite-client-1.0.8/test/test_study_inputs.py
--rw-rw-rw-   0        0        0     1690 2024-02-29 13:16:04.000000 spacestudio-satellite-client-1.0.8/test/test_study_parameters.py
--rw-rw-rw-   0        0        0     1710 2024-02-29 13:16:04.000000 spacestudio-satellite-client-1.0.8/test/test_tab.py
--rw-rw-rw-   0        0        0     1474 2024-02-29 13:16:04.000000 spacestudio-satellite-client-1.0.8/test/test_third_body_perturbation.py
--rw-rw-rw-   0        0        0      776 2024-02-29 13:16:04.000000 spacestudio-satellite-client-1.0.8/test/test_thrust_arcs_position.py
--rw-rw-rw-   0        0        0     1457 2024-02-29 13:16:04.000000 spacestudio-satellite-client-1.0.8/test/test_timeline_slot.py
+drwxrwxrwx   0        0        0        0 2024-02-29 14:26:34.790605 spacestudio-satellite-client-1.0.9/
+-rw-rw-rw-   0        0        0      570 2024-02-29 14:26:34.790605 spacestudio-satellite-client-1.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0    11988 2024-02-29 14:24:10.000000 spacestudio-satellite-client-1.0.9/README.md
+-rw-rw-rw-   0        0        0     2020 2024-02-29 14:24:10.000000 spacestudio-satellite-client-1.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0       76 2024-02-29 14:26:34.793609 spacestudio-satellite-client-1.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1414 2024-02-29 14:24:10.000000 spacestudio-satellite-client-1.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-02-29 14:26:34.540655 spacestudio-satellite-client-1.0.9/spacestudio_satellite_client/
+-rw-rw-rw-   0        0        0     7406 2024-02-29 14:24:10.000000 spacestudio-satellite-client-1.0.9/spacestudio_satellite_client/__init__.py
+drwxrwxrwx   0        0        0        0 2024-02-29 14:26:34.575039 spacestudio-satellite-client-1.0.9/spacestudio_satellite_client/api/
+-rw-rw-rw-   0        0        0      744 2024-02-29 14:24:10.000000 spacestudio-satellite-client-1.0.9/spacestudio_satellite_client/api/__init__.py
+-rw-rw-rw-   0        0        0    30710 2024-02-29 14:24:10.000000 spacestudio-satellite-client-1.0.9/spacestudio_satellite_client/api/announcement_api.py
+-rw-rw-rw-   0        0        0    19800 2024-02-29 14:24:10.000000 spacestudio-satellite-client-1.0.9/spacestudio_satellite_client/api/computations_api.py
+-rw-rw-rw-   0        0        0    21182 2024-02-29 14:24:10.000000 spacestudio-satellite-client-1.0.9/spacestudio_satellite_client/api/notification_api.py
+-rw-rw-rw-   0        0        0    51641 2024-02-29 14:24:10.000000 spacestudio-satellite-client-1.0.9/spacestudio_satellite_client/api/orbits_api.py
+-rw-rw-rw-   0        0        0    52103 2024-02-29 14:24:10.000000 spacestudio-satellite-client-1.0.9/spacestudio_satellite_client/api/platforms_api.py
+-rw-rw-rw-   0        0        0    53440 2024-02-29 14:24:10.000000 spacestudio-satellite-client-1.0.9/spacestudio_satellite_client/api/propulsion_systems_api.py
+-rw-rw-rw-   0        0        0    72103 2024-02-29 14:24:10.000000 spacestudio-satellite-client-1.0.9/spacestudio_satellite_client/api/scenarios_api.py
+-rw-rw-rw-   0        0        0    53736 2024-02-29 14:24:10.000000 spacestudio-satellite-client-1.0.9/spacestudio_satellite_client/api/spacecraft_geometries_api.py
+-rw-rw-rw-   0        0        0    77009 2024-02-29 14:24:10.000000 spacestudio-satellite-client-1.0.9/spacestudio_satellite_client/api/studies_api.py
+-rw-rw-rw-   0        0        0    25897 2024-02-29 14:24:10.000000 spacestudio-satellite-client-1.0.9/spacestudio_satellite_client/api_client.py
+-rw-rw-rw-   0        0        0      652 2024-02-29 14:24:10.000000 spacestudio-satellite-client-1.0.9/spacestudio_satellite_client/api_response.py
+-rw-rw-rw-   0        0        0    14838 2024-02-29 14:24:10.000000 spacestudio-satellite-client-1.0.9/spacestudio_satellite_client/configuration.py
+-rw-rw-rw-   0        0        0     5994 2024-02-29 14:24:10.000000 spacestudio-satellite-client-1.0.9/spacestudio_satellite_client/exceptions.py
+drwxrwxrwx   0        0        0        0 2024-02-29 14:26:34.659606 spacestudio-satellite-client-1.0.9/spacestudio_satellite_client/models/
+-rw-rw-rw-   0        0        0     6040 2024-02-29 14:24:10.000000 spacestudio-satellite-client-1.0.9/spacestudio_satellite_client/models/__init__.py
+-rw-rw-rw-   0        0        0     5157 2024-02-29 14:24:09.000000 spacestudio-satellite-client-1.0.9/spacestudio_satellite_client/models/advanced_orbit_parameters.py
+-rw-rw-rw-   0        0        0     3440 2024-02-29 14:24:09.000000 spacestudio-satellite-client-1.0.9/spacestudio_satellite_client/models/analytical_study_parameters.py
+-rw-rw-rw-   0        0        0     3302 2024-02-29 14:24:09.000000 spacestudio-satellite-client-1.0.9/spacestudio_satellite_client/models/announcement.py
+-rw-rw-rw-   0        0        0     2960 2024-02-29 14:24:09.000000 spacestudio-satellite-client-1.0.9/spacestudio_satellite_client/models/baseline_configuration.py
+-rw-rw-rw-   0        0        0     2873 2024-02-29 14:24:09.000000 spacestudio-satellite-client-1.0.9/spacestudio_satellite_client/models/circular_altitude_orbit_parameters.py
+-rw-rw-rw-   0        0        0     3119 2024-02-29 14:24:09.000000 spacestudio-satellite-client-1.0.9/spacestudio_satellite_client/models/circular_ground_track_repeated_orbit_parameters.py
+-rw-rw-rw-   0        0        0     4574 2024-02-29 14:24:09.000000 spacestudio-satellite-client-1.0.9/spacestudio_satellite_client/models/comparison_item.py
+-rw-rw-rw-   0        0        0     4578 2024-02-29 14:24:09.000000 spacestudio-satellite-client-1.0.9/spacestudio_satellite_client/models/comparison_item1.py
+-rw-rw-rw-   0        0        0     4516 2024-02-29 14:24:09.000000 spacestudio-satellite-client-1.0.9/spacestudio_satellite_client/models/computation.py
+-rw-rw-rw-   0        0        0      794 2024-02-29 14:24:09.000000 spacestudio-satellite-client-1.0.9/spacestudio_satellite_client/models/computation_mode.py
+-rw-rw-rw-   0        0        0     4031 2024-02-29 14:24:09.000000 spacestudio-satellite-client-1.0.9/spacestudio_satellite_client/models/computation_outputs.py
+-rw-rw-rw-   0        0        0      890 2024-02-29 14:24:09.000000 spacestudio-satellite-client-1.0.9/spacestudio_satellite_client/models/computation_status.py
+-rw-rw-rw-   0        0        0      794 2024-02-29 14:24:09.000000 spacestudio-satellite-client-1.0.9/spacestudio_satellite_client/models/computation_type.py
+-rw-rw-rw-   0        0        0     2736 2024-02-29 14:24:09.000000 spacestudio-satellite-client-1.0.9/spacestudio_satellite_client/models/context_outputs.py
+-rw-rw-rw-   0        0        0     2476 2024-02-29 14:24:09.000000 spacestudio-satellite-client-1.0.9/spacestudio_satellite_client/models/deorbitation.py
+-rw-rw-rw-   0        0        0     4590 2024-02-29 14:24:09.000000 spacestudio-satellite-client-1.0.9/spacestudio_satellite_client/models/display_configuration.py
+-rw-rw-rw-   0        0        0     3684 2024-02-29 14:24:09.000000 spacestudio-satellite-client-1.0.9/spacestudio_satellite_client/models/display_configuration_comparison_overview.py
+-rw-rw-rw-   0        0        0     2885 2024-02-29 14:24:09.000000 spacestudio-satellite-client-1.0.9/spacestudio_satellite_client/models/drag_perturbation.py
+-rw-rw-rw-   0        0        0     2621 2024-02-29 14:24:09.000000 spacestudio-satellite-client-1.0.9/spacestudio_satellite_client/models/duplicate_scenario_request.py
+-rw-rw-rw-   0        0        0      818 2024-02-29 14:24:09.000000 spacestudio-satellite-client-1.0.9/spacestudio_satellite_client/models/earth_potential_configuration.py
+-rw-rw-rw-   0        0        0     3545 2024-02-29 14:24:09.000000 spacestudio-satellite-client-1.0.9/spacestudio_satellite_client/models/earth_potential_perturbation.py
+-rw-rw-rw-   0        0        0     3175 2024-02-29 14:24:09.000000 spacestudio-satellite-client-1.0.9/spacestudio_satellite_client/models/elliptical_ground_track_repeated_eccentricity_orbit_parameters.py
+-rw-rw-rw-   0        0        0     3222 2024-02-29 14:24:09.000000 spacestudio-satellite-client-1.0.9/spacestudio_satellite_client/models/elliptical_perigee_alt_apogee_alt_orbit_parameters.py
+-rw-rw-rw-   0        0        0     2999 2024-02-29 14:24:09.000000 spacestudio-satellite-client-1.0.9/spacestudio_satellite_client/models/elliptical_perigee_alt_eccentricity_orbit_parameters.py
+-rw-rw-rw-   0        0        0     2699 2024-02-29 14:24:09.000000 spacestudio-satellite-client-1.0.9/spacestudio_satellite_client/models/elliptical_sma_eccentricity_orbit_parameters.py
+-rw-rw-rw-   0        0        0     3457 2024-02-29 14:24:09.000000 spacestudio-satellite-client-1.0.9/spacestudio_satellite_client/models/leo_station_keeping.py
+-rw-rw-rw-   0        0        0     4743 2024-02-29 14:24:09.000000 spacestudio-satellite-client-1.0.9/spacestudio_satellite_client/models/maneuver.py
+-rw-rw-rw-   0        0        0     4569 2024-02-29 14:24:09.000000 spacestudio-satellite-client-1.0.9/spacestudio_satellite_client/models/maneuver_timeline_slot.py
+-rw-rw-rw-   0        0        0     6661 2024-02-29 14:24:09.000000 spacestudio-satellite-client-1.0.9/spacestudio_satellite_client/models/maneuvering_strategy.py
+-rw-rw-rw-   0        0        0     3805 2024-02-29 14:24:09.000000 spacestudio-satellite-client-1.0.9/spacestudio_satellite_client/models/notification.py
+-rw-rw-rw-   0        0        0     2723 2024-02-29 14:24:09.000000 spacestudio-satellite-client-1.0.9/spacestudio_satellite_client/models/notification_content.py
+-rw-rw-rw-   0        0        0     2815 2024-02-29 14:24:09.000000 spacestudio-satellite-client-1.0.9/spacestudio_satellite_client/models/numerical_ephemeris.py
+-rw-rw-rw-   0        0        0     5113 2024-02-29 14:24:09.000000 spacestudio-satellite-client-1.0.9/spacestudio_satellite_client/models/numerical_outputs_configuration.py
+-rw-rw-rw-   0        0        0     5429 2024-02-29 14:24:09.000000 spacestudio-satellite-client-1.0.9/spacestudio_satellite_client/models/numerical_study_parameters.py
+-rw-rw-rw-   0        0        0     4704 2024-02-29 14:24:09.000000 spacestudio-satellite-client-1.0.9/spacestudio_satellite_client/models/orbit.py
+-rw-rw-rw-   0        0        0     3349 2024-02-29 14:24:09.000000 spacestudio-satellite-client-1.0.9/spacestudio_satellite_client/models/orbit_parameters.py
+-rw-rw-rw-   0        0        0     3621 2024-02-29 14:24:09.000000 spacestudio-satellite-client-1.0.9/spacestudio_satellite_client/models/orbit_phasing.py
+-rw-rw-rw-   0        0        0     2734 2024-02-29 14:24:09.000000 spacestudio-satellite-client-1.0.9/spacestudio_satellite_client/models/orbit_propagation.py
+-rw-rw-rw-   0        0        0     2969 2024-02-29 14:24:09.000000 spacestudio-satellite-client-1.0.9/spacestudio_satellite_client/models/orbit_timeline_slot.py
+-rw-rw-rw-   0        0        0     2488 2024-02-29 14:24:09.000000 spacestudio-satellite-client-1.0.9/spacestudio_satellite_client/models/orbital_transfer.py
+-rw-rw-rw-   0        0        0     2802 2024-02-29 14:24:09.000000 spacestudio-satellite-client-1.0.9/spacestudio_satellite_client/models/payload.py
+-rw-rw-rw-   0        0        0     4185 2024-02-29 14:24:09.000000 spacestudio-satellite-client-1.0.9/spacestudio_satellite_client/models/perturbation.py
+-rw-rw-rw-   0        0        0      843 2024-02-29 14:24:09.000000 spacestudio-satellite-client-1.0.9/spacestudio_satellite_client/models/perturbation_type.py
+-rw-rw-rw-   0        0        0     4464 2024-02-29 14:24:09.000000 spacestudio-satellite-client-1.0.9/spacestudio_satellite_client/models/platform.py
+-rw-rw-rw-   0        0        0     3510 2024-02-29 14:24:09.000000 spacestudio-satellite-client-1.0.9/spacestudio_satellite_client/models/plot.py
+-rw-rw-rw-   0        0        0     6472 2024-02-29 14:24:09.000000 spacestudio-satellite-client-1.0.9/spacestudio_satellite_client/models/propulsion_system.py
+-rw-rw-rw-   0        0        0     5454 2024-02-29 14:24:09.000000 spacestudio-satellite-client-1.0.9/spacestudio_satellite_client/models/raan_phasing.py
+-rw-rw-rw-   0        0        0     3731 2024-02-29 14:24:09.000000 spacestudio-satellite-client-1.0.9/spacestudio_satellite_client/models/scenario.py
+-rw-rw-rw-   0        0        0     8722 2024-02-29 14:24:09.000000 spacestudio-satellite-client-1.0.9/spacestudio_satellite_client/models/scenario_baseline.py
+-rw-rw-rw-   0        0        0     3360 2024-02-29 14:24:09.000000 spacestudio-satellite-client-1.0.9/spacestudio_satellite_client/models/simulation_configuration.py
+-rw-rw-rw-   0        0        0     6152 2024-02-29 14:24:09.000000 spacestudio-satellite-client-1.0.9/spacestudio_satellite_client/models/single_satellite_analytical_computation_outputs.py
+-rw-rw-rw-   0        0        0     5728 2024-02-29 14:24:09.000000 spacestudio-satellite-client-1.0.9/spacestudio_satellite_client/models/single_satellite_numerical_computation_outputs.py
+-rw-rw-rw-   0        0        0     2659 2024-02-29 14:24:09.000000 spacestudio-satellite-client-1.0.9/spacestudio_satellite_client/models/solar_radiation_pressure_perturbation.py
+-rw-rw-rw-   0        0        0    15511 2024-02-29 14:24:09.000000 spacestudio-satellite-client-1.0.9/spacestudio_satellite_client/models/spacecraft_geometry.py
+-rw-rw-rw-   0        0        0     6204 2024-02-29 14:24:09.000000 spacestudio-satellite-client-1.0.9/spacestudio_satellite_client/models/study.py
+-rw-rw-rw-   0        0        0     3966 2024-02-29 14:24:09.000000 spacestudio-satellite-client-1.0.9/spacestudio_satellite_client/models/study_computation.py
+-rw-rw-rw-   0        0        0     7407 2024-02-29 14:24:09.000000 spacestudio-satellite-client-1.0.9/spacestudio_satellite_client/models/study_inputs.py
+-rw-rw-rw-   0        0        0     4654 2024-02-29 14:24:09.000000 spacestudio-satellite-client-1.0.9/spacestudio_satellite_client/models/study_parameters.py
+-rw-rw-rw-   0        0        0     3171 2024-02-29 14:24:09.000000 spacestudio-satellite-client-1.0.9/spacestudio_satellite_client/models/tab.py
+-rw-rw-rw-   0        0        0     2607 2024-02-29 14:24:09.000000 spacestudio-satellite-client-1.0.9/spacestudio_satellite_client/models/third_body_perturbation.py
+-rw-rw-rw-   0        0        0     1217 2024-02-29 14:24:09.000000 spacestudio-satellite-client-1.0.9/spacestudio_satellite_client/models/thrust_arcs_position.py
+-rw-rw-rw-   0        0        0     4628 2024-02-29 14:24:09.000000 spacestudio-satellite-client-1.0.9/spacestudio_satellite_client/models/timeline_slot.py
+-rw-rw-rw-   0        0        0        0 2024-02-29 14:24:10.000000 spacestudio-satellite-client-1.0.9/spacestudio_satellite_client/py.typed
+-rw-rw-rw-   0        0        0     9268 2024-02-29 14:24:10.000000 spacestudio-satellite-client-1.0.9/spacestudio_satellite_client/rest.py
+drwxrwxrwx   0        0        0        0 2024-02-29 14:26:34.788604 spacestudio-satellite-client-1.0.9/spacestudio_satellite_client.egg-info/
+-rw-rw-rw-   0        0        0      570 2024-02-29 14:26:34.000000 spacestudio-satellite-client-1.0.9/spacestudio_satellite_client.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     7423 2024-02-29 14:26:34.000000 spacestudio-satellite-client-1.0.9/spacestudio_satellite_client.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-02-29 14:26:34.000000 spacestudio-satellite-client-1.0.9/spacestudio_satellite_client.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       76 2024-02-29 14:26:34.000000 spacestudio-satellite-client-1.0.9/spacestudio_satellite_client.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       29 2024-02-29 14:26:34.000000 spacestudio-satellite-client-1.0.9/spacestudio_satellite_client.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-02-29 14:26:34.786609 spacestudio-satellite-client-1.0.9/test/
+-rw-rw-rw-   0        0        0     1798 2024-02-29 13:16:03.000000 spacestudio-satellite-client-1.0.9/test/test_advanced_orbit_parameters.py
+-rw-rw-rw-   0        0        0     1522 2024-02-29 13:16:03.000000 spacestudio-satellite-client-1.0.9/test/test_analytical_study_parameters.py
+-rw-rw-rw-   0        0        0     1692 2024-02-29 13:16:03.000000 spacestudio-satellite-client-1.0.9/test/test_announcement.py
+-rw-rw-rw-   0        0        0     1113 2024-02-29 13:16:03.000000 spacestudio-satellite-client-1.0.9/test/test_announcement_api.py
+-rw-rw-rw-   0        0        0     1860 2024-02-29 13:16:03.000000 spacestudio-satellite-client-1.0.9/test/test_baseline_configuration.py
+-rw-rw-rw-   0        0        0     1628 2024-02-29 13:16:03.000000 spacestudio-satellite-client-1.0.9/test/test_circular_altitude_orbit_parameters.py
+-rw-rw-rw-   0        0        0     1809 2024-02-29 13:16:03.000000 spacestudio-satellite-client-1.0.9/test/test_circular_ground_track_repeated_orbit_parameters.py
+-rw-rw-rw-   0        0        0     1812 2024-02-29 13:16:03.000000 spacestudio-satellite-client-1.0.9/test/test_comparison_item.py
+-rw-rw-rw-   0        0        0     1824 2024-02-29 13:16:03.000000 spacestudio-satellite-client-1.0.9/test/test_comparison_item1.py
+-rw-rw-rw-   0        0        0     2413 2024-02-29 13:16:03.000000 spacestudio-satellite-client-1.0.9/test/test_computation.py
+-rw-rw-rw-   0        0        0      754 2024-02-29 13:16:03.000000 spacestudio-satellite-client-1.0.9/test/test_computation_mode.py
+-rw-rw-rw-   0        0        0     1473 2024-02-29 13:16:03.000000 spacestudio-satellite-client-1.0.9/test/test_computation_outputs.py
+-rw-rw-rw-   0        0        0      768 2024-02-29 13:16:03.000000 spacestudio-satellite-client-1.0.9/test/test_computation_status.py
+-rw-rw-rw-   0        0        0      754 2024-02-29 13:16:03.000000 spacestudio-satellite-client-1.0.9/test/test_computation_type.py
+-rw-rw-rw-   0        0        0      992 2024-02-29 13:16:03.000000 spacestudio-satellite-client-1.0.9/test/test_computations_api.py
+-rw-rw-rw-   0        0        0     1436 2024-02-29 13:16:03.000000 spacestudio-satellite-client-1.0.9/test/test_context_outputs.py
+-rw-rw-rw-   0        0        0     1364 2024-02-29 13:16:03.000000 spacestudio-satellite-client-1.0.9/test/test_deorbitation.py
+-rw-rw-rw-   0        0        0     3991 2024-02-29 13:16:03.000000 spacestudio-satellite-client-1.0.9/test/test_display_configuration.py
+-rw-rw-rw-   0        0        0     2186 2024-02-29 13:16:03.000000 spacestudio-satellite-client-1.0.9/test/test_display_configuration_comparison_overview.py
+-rw-rw-rw-   0        0        0     1455 2024-02-29 13:16:03.000000 spacestudio-satellite-client-1.0.9/test/test_drag_perturbation.py
+-rw-rw-rw-   0        0        0     1558 2024-02-29 13:16:03.000000 spacestudio-satellite-client-1.0.9/test/test_duplicate_scenario_request.py
+-rw-rw-rw-   0        0        0      839 2024-02-29 13:16:03.000000 spacestudio-satellite-client-1.0.9/test/test_earth_potential_configuration.py
+-rw-rw-rw-   0        0        0     1694 2024-02-29 13:16:03.000000 spacestudio-satellite-client-1.0.9/test/test_earth_potential_perturbation.py
+-rw-rw-rw-   0        0        0     1978 2024-02-29 13:16:03.000000 spacestudio-satellite-client-1.0.9/test/test_elliptical_ground_track_repeated_eccentricity_orbit_parameters.py
+-rw-rw-rw-   0        0        0     1836 2024-02-29 13:16:03.000000 spacestudio-satellite-client-1.0.9/test/test_elliptical_perigee_alt_apogee_alt_orbit_parameters.py
+-rw-rw-rw-   0        0        0     1830 2024-02-29 13:16:03.000000 spacestudio-satellite-client-1.0.9/test/test_elliptical_perigee_alt_eccentricity_orbit_parameters.py
+-rw-rw-rw-   0        0        0     1704 2024-02-29 13:16:03.000000 spacestudio-satellite-client-1.0.9/test/test_elliptical_sma_eccentricity_orbit_parameters.py
+-rw-rw-rw-   0        0        0     1590 2024-02-29 13:16:03.000000 spacestudio-satellite-client-1.0.9/test/test_leo_station_keeping.py
+-rw-rw-rw-   0        0        0     1358 2024-02-29 13:16:03.000000 spacestudio-satellite-client-1.0.9/test/test_maneuver.py
+-rw-rw-rw-   0        0        0     4709 2024-02-29 13:16:03.000000 spacestudio-satellite-client-1.0.9/test/test_maneuver_timeline_slot.py
+-rw-rw-rw-   0        0        0     2176 2024-02-29 13:16:03.000000 spacestudio-satellite-client-1.0.9/test/test_maneuvering_strategy.py
+-rw-rw-rw-   0        0        0     1990 2024-02-29 13:16:03.000000 spacestudio-satellite-client-1.0.9/test/test_notification.py
+-rw-rw-rw-   0        0        0      977 2024-02-29 13:16:03.000000 spacestudio-satellite-client-1.0.9/test/test_notification_api.py
+-rw-rw-rw-   0        0        0     1536 2024-02-29 13:16:03.000000 spacestudio-satellite-client-1.0.9/test/test_notification_content.py
+-rw-rw-rw-   0        0        0     1660 2024-02-29 13:16:03.000000 spacestudio-satellite-client-1.0.9/test/test_numerical_ephemeris.py
+-rw-rw-rw-   0        0        0     1945 2024-02-29 13:16:03.000000 spacestudio-satellite-client-1.0.9/test/test_numerical_outputs_configuration.py
+-rw-rw-rw-   0        0        0     3236 2024-02-29 13:16:03.000000 spacestudio-satellite-client-1.0.9/test/test_numerical_study_parameters.py
+-rw-rw-rw-   0        0        0     2091 2024-02-29 13:16:03.000000 spacestudio-satellite-client-1.0.9/test/test_orbit.py
+-rw-rw-rw-   0        0        0     1455 2024-02-29 13:16:03.000000 spacestudio-satellite-client-1.0.9/test/test_orbit_parameters.py
+-rw-rw-rw-   0        0        0     1563 2024-02-29 13:16:03.000000 spacestudio-satellite-client-1.0.9/test/test_orbit_phasing.py
+-rw-rw-rw-   0        0        0     1446 2024-02-29 13:16:03.000000 spacestudio-satellite-client-1.0.9/test/test_orbit_propagation.py
+-rw-rw-rw-   0        0        0     2394 2024-02-29 13:16:03.000000 spacestudio-satellite-client-1.0.9/test/test_orbit_timeline_slot.py
+-rw-rw-rw-   0        0        0     1401 2024-02-29 13:16:03.000000 spacestudio-satellite-client-1.0.9/test/test_orbital_transfer.py
+-rw-rw-rw-   0        0        0     1284 2024-02-29 13:16:03.000000 spacestudio-satellite-client-1.0.9/test/test_orbits_api.py
+-rw-rw-rw-   0        0        0     1383 2024-02-29 13:16:03.000000 spacestudio-satellite-client-1.0.9/test/test_payload.py
+-rw-rw-rw-   0        0        0     1394 2024-02-29 13:16:03.000000 spacestudio-satellite-client-1.0.9/test/test_perturbation.py
+-rw-rw-rw-   0        0        0      761 2024-02-29 13:16:03.000000 spacestudio-satellite-client-1.0.9/test/test_perturbation_type.py
+-rw-rw-rw-   0        0        0     1692 2024-02-29 13:16:03.000000 spacestudio-satellite-client-1.0.9/test/test_platform.py
+-rw-rw-rw-   0        0        0     1344 2024-02-29 13:16:03.000000 spacestudio-satellite-client-1.0.9/test/test_platforms_api.py
+-rw-rw-rw-   0        0        0     1477 2024-02-29 13:16:03.000000 spacestudio-satellite-client-1.0.9/test/test_plot.py
+-rw-rw-rw-   0        0        0     2018 2024-02-29 13:16:03.000000 spacestudio-satellite-client-1.0.9/test/test_propulsion_system.py
+-rw-rw-rw-   0        0        0     1515 2024-02-29 13:16:03.000000 spacestudio-satellite-client-1.0.9/test/test_propulsion_systems_api.py
+-rw-rw-rw-   0        0        0     1891 2024-02-29 13:16:03.000000 spacestudio-satellite-client-1.0.9/test/test_raan_phasing.py
+-rw-rw-rw-   0        0        0     6570 2024-02-29 13:16:03.000000 spacestudio-satellite-client-1.0.9/test/test_scenario.py
+-rw-rw-rw-   0        0        0     5853 2024-02-29 13:16:03.000000 spacestudio-satellite-client-1.0.9/test/test_scenario_baseline.py
+-rw-rw-rw-   0        0        0     1611 2024-02-29 13:16:03.000000 spacestudio-satellite-client-1.0.9/test/test_scenarios_api.py
+-rw-rw-rw-   0        0        0     1597 2024-02-29 13:16:03.000000 spacestudio-satellite-client-1.0.9/test/test_simulation_configuration.py
+-rw-rw-rw-   0        0        0     2431 2024-02-29 13:16:03.000000 spacestudio-satellite-client-1.0.9/test/test_single_satellite_analytical_computation_outputs.py
+-rw-rw-rw-   0        0        0     2606 2024-02-29 13:16:03.000000 spacestudio-satellite-client-1.0.9/test/test_single_satellite_numerical_computation_outputs.py
+-rw-rw-rw-   0        0        0     1631 2024-02-29 13:16:03.000000 spacestudio-satellite-client-1.0.9/test/test_solar_radiation_pressure_perturbation.py
+-rw-rw-rw-   0        0        0     1566 2024-02-29 13:16:03.000000 spacestudio-satellite-client-1.0.9/test/test_spacecraft_geometries_api.py
+-rw-rw-rw-   0        0        0     3509 2024-02-29 13:16:03.000000 spacestudio-satellite-client-1.0.9/test/test_spacecraft_geometry.py
+-rw-rw-rw-   0        0        0     1614 2024-02-29 13:16:04.000000 spacestudio-satellite-client-1.0.9/test/test_studies_api.py
+-rw-rw-rw-   0        0        0    11380 2024-02-29 13:16:04.000000 spacestudio-satellite-client-1.0.9/test/test_study.py
+-rw-rw-rw-   0        0        0     3974 2024-02-29 13:16:04.000000 spacestudio-satellite-client-1.0.9/test/test_study_computation.py
+-rw-rw-rw-   0        0        0     7220 2024-02-29 13:16:04.000000 spacestudio-satellite-client-1.0.9/test/test_study_inputs.py
+-rw-rw-rw-   0        0        0     1690 2024-02-29 13:16:04.000000 spacestudio-satellite-client-1.0.9/test/test_study_parameters.py
+-rw-rw-rw-   0        0        0     1710 2024-02-29 13:16:04.000000 spacestudio-satellite-client-1.0.9/test/test_tab.py
+-rw-rw-rw-   0        0        0     1474 2024-02-29 13:16:04.000000 spacestudio-satellite-client-1.0.9/test/test_third_body_perturbation.py
+-rw-rw-rw-   0        0        0      776 2024-02-29 13:16:04.000000 spacestudio-satellite-client-1.0.9/test/test_thrust_arcs_position.py
+-rw-rw-rw-   0        0        0     1457 2024-02-29 13:16:04.000000 spacestudio-satellite-client-1.0.9/test/test_timeline_slot.py
```

### Comparing `spacestudio-satellite-client-1.0.8/PKG-INFO` & `spacestudio-satellite-client-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spacestudio-satellite-client
-Version: 1.0.8
+Version: 1.0.9
 Summary: Spacestudio API documentation
 Home-page: 
 Author: OpenAPI Generator community
 Author-email: team@openapitools.org
 Keywords: OpenAPI,OpenAPI-Generator,Spacestudio API documentation
 Description-Content-Type: text/markdown
 Requires-Dist: urllib3<2.1.0,>=1.25.3
```

### Comparing `spacestudio-satellite-client-1.0.8/README.md` & `spacestudio-satellite-client-1.0.9/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # spacestudio-satellite-client
 No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
 - API version: 1.0.1
-- Package version: 1.0.8
+- Package version: 1.0.9
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 
 ## Requirements.
 
 Python 3.7+
 
 ## Installation & Usage
```

### Comparing `spacestudio-satellite-client-1.0.8/pyproject.toml` & `spacestudio-satellite-client-1.0.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "spacestudio_satellite_client"
-version = "1.0.8"
+version = "1.0.9"
 description = "Spacestudio API documentation"
 authors = ["OpenAPI Generator Community <team@openapitools.org>"]
 license = "NoLicense"
 readme = "README.md"
 repository = "https://github.com/GIT_USER_ID/GIT_REPO_ID"
 keywords = ["OpenAPI", "OpenAPI-Generator", "Spacestudio API documentation"]
 include = ["spacestudio_satellite_client/py.typed"]
```

### Comparing `spacestudio-satellite-client-1.0.8/setup.py` & `spacestudio-satellite-client-1.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
 NAME = "spacestudio-satellite-client"
-VERSION = "1.0.8"
+VERSION = "1.0.9"
 PYTHON_REQUIRES = ">=3.7"
 REQUIRES = [
     "urllib3 >= 1.25.3, < 2.1.0",
     "python-dateutil",
     "pydantic >= 2",
     "typing-extensions >= 4.7.1",
 ]
```

### Comparing `spacestudio-satellite-client-1.0.8/spacestudio_satellite_client/__init__.py` & `spacestudio-satellite-client-1.0.9/spacestudio_satellite_client/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     The version of the OpenAPI document: 1.0.1
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
-__version__ = "1.0.8"
+__version__ = "1.0.9"
 
 # import apis into sdk package
 from spacestudio_satellite_client.api.announcement_api import AnnouncementApi
 from spacestudio_satellite_client.api.computations_api import ComputationsApi
 from spacestudio_satellite_client.api.notification_api import NotificationApi
 from spacestudio_satellite_client.api.orbits_api import OrbitsApi
 from spacestudio_satellite_client.api.platforms_api import PlatformsApi
```

### Comparing `spacestudio-satellite-client-1.0.8/spacestudio_satellite_client/api/__init__.py` & `spacestudio-satellite-client-1.0.9/spacestudio_satellite_client/api/__init__.py`

 * *Files identical despite different names*

### Comparing `spacestudio-satellite-client-1.0.8/spacestudio_satellite_client/api/announcement_api.py` & `spacestudio-satellite-client-1.0.9/spacestudio_satellite_client/api/announcement_api.py`

 * *Files identical despite different names*

### Comparing `spacestudio-satellite-client-1.0.8/spacestudio_satellite_client/api/computations_api.py` & `spacestudio-satellite-client-1.0.9/spacestudio_satellite_client/api/computations_api.py`

 * *Files identical despite different names*

### Comparing `spacestudio-satellite-client-1.0.8/spacestudio_satellite_client/api/notification_api.py` & `spacestudio-satellite-client-1.0.9/spacestudio_satellite_client/api/notification_api.py`

 * *Files identical despite different names*

### Comparing `spacestudio-satellite-client-1.0.8/spacestudio_satellite_client/api/orbits_api.py` & `spacestudio-satellite-client-1.0.9/spacestudio_satellite_client/api/orbits_api.py`

 * *Files identical despite different names*

### Comparing `spacestudio-satellite-client-1.0.8/spacestudio_satellite_client/api/platforms_api.py` & `spacestudio-satellite-client-1.0.9/spacestudio_satellite_client/api/platforms_api.py`

 * *Files identical despite different names*

### Comparing `spacestudio-satellite-client-1.0.8/spacestudio_satellite_client/api/propulsion_systems_api.py` & `spacestudio-satellite-client-1.0.9/spacestudio_satellite_client/api/propulsion_systems_api.py`

 * *Files identical despite different names*

### Comparing `spacestudio-satellite-client-1.0.8/spacestudio_satellite_client/api/scenarios_api.py` & `spacestudio-satellite-client-1.0.9/spacestudio_satellite_client/api/scenarios_api.py`

 * *Files identical despite different names*

### Comparing `spacestudio-satellite-client-1.0.8/spacestudio_satellite_client/api/spacecraft_geometries_api.py` & `spacestudio-satellite-client-1.0.9/spacestudio_satellite_client/api/spacecraft_geometries_api.py`

 * *Files identical despite different names*

### Comparing `spacestudio-satellite-client-1.0.8/spacestudio_satellite_client/api/studies_api.py` & `spacestudio-satellite-client-1.0.9/spacestudio_satellite_client/api/studies_api.py`

 * *Files identical despite different names*

### Comparing `spacestudio-satellite-client-1.0.8/spacestudio_satellite_client/api_client.py` & `spacestudio-satellite-client-1.0.9/spacestudio_satellite_client/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -83,15 +83,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/1.0.8/python'
+        self.user_agent = 'OpenAPI-Generator/1.0.9/python'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         pass
```

### Comparing `spacestudio-satellite-client-1.0.8/spacestudio_satellite_client/api_response.py` & `spacestudio-satellite-client-1.0.9/spacestudio_satellite_client/api_response.py`

 * *Files identical despite different names*

### Comparing `spacestudio-satellite-client-1.0.8/spacestudio_satellite_client/configuration.py` & `spacestudio-satellite-client-1.0.9/spacestudio_satellite_client/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -374,15 +374,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: 1.0.1\n"\
-               "SDK Package Version: 1.0.8".\
+               "SDK Package Version: 1.0.9".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `spacestudio-satellite-client-1.0.8/spacestudio_satellite_client/exceptions.py` & `spacestudio-satellite-client-1.0.9/spacestudio_satellite_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `spacestudio-satellite-client-1.0.8/spacestudio_satellite_client/models/__init__.py` & `spacestudio-satellite-client-1.0.9/spacestudio_satellite_client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `spacestudio-satellite-client-1.0.8/spacestudio_satellite_client/models/advanced_orbit_parameters.py` & `spacestudio-satellite-client-1.0.9/spacestudio_satellite_client/models/advanced_orbit_parameters.py`

 * *Files identical despite different names*

### Comparing `spacestudio-satellite-client-1.0.8/spacestudio_satellite_client/models/analytical_study_parameters.py` & `spacestudio-satellite-client-1.0.9/spacestudio_satellite_client/models/analytical_study_parameters.py`

 * *Files identical despite different names*

### Comparing `spacestudio-satellite-client-1.0.8/spacestudio_satellite_client/models/announcement.py` & `spacestudio-satellite-client-1.0.9/spacestudio_satellite_client/models/announcement.py`

 * *Files identical despite different names*

### Comparing `spacestudio-satellite-client-1.0.8/spacestudio_satellite_client/models/baseline_configuration.py` & `spacestudio-satellite-client-1.0.9/spacestudio_satellite_client/models/baseline_configuration.py`

 * *Files identical despite different names*

### Comparing `spacestudio-satellite-client-1.0.8/spacestudio_satellite_client/models/circular_altitude_orbit_parameters.py` & `spacestudio-satellite-client-1.0.9/spacestudio_satellite_client/models/circular_altitude_orbit_parameters.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,24 +13,24 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import Field, StrictFloat, StrictInt
+from pydantic import BaseModel, Field, StrictFloat, StrictInt, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional, Union
-from spacestudio_satellite_client.models.orbit_parameters import OrbitParameters
 from typing import Optional, Set
 from typing_extensions import Self
 
-class CircularAltitudeOrbitParameters(OrbitParameters):
+class CircularAltitudeOrbitParameters(BaseModel):
     """
     CircularAltitudeOrbitParameters
     """ # noqa: E501
+    parameters_type: Optional[StrictStr] = Field(default=None, alias="parametersType")
     altitude: Optional[Union[StrictFloat, StrictInt]] = Field(default=None, description="The orbit altitude (in meters)")
     __properties: ClassVar[List[str]] = ["parametersType", "altitude"]
 
     model_config = {
         "populate_by_name": True,
         "validate_assignment": True,
         "protected_namespaces": (),
```

### Comparing `spacestudio-satellite-client-1.0.8/spacestudio_satellite_client/models/circular_ground_track_repeated_orbit_parameters.py` & `spacestudio-satellite-client-1.0.9/spacestudio_satellite_client/models/circular_ground_track_repeated_orbit_parameters.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,24 +13,24 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import Field, StrictFloat, StrictInt
+from pydantic import BaseModel, Field, StrictFloat, StrictInt, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional, Union
-from spacestudio_satellite_client.models.orbit_parameters import OrbitParameters
 from typing import Optional, Set
 from typing_extensions import Self
 
-class CircularGroundTrackRepeatedOrbitParameters(OrbitParameters):
+class CircularGroundTrackRepeatedOrbitParameters(BaseModel):
     """
     CircularGroundTrackRepeatedOrbitParameters
     """ # noqa: E501
+    parameters_type: Optional[StrictStr] = Field(default=None, alias="parametersType")
     n: Optional[Union[StrictFloat, StrictInt]] = Field(default=None, description="//TODO")
     p: Optional[Union[StrictFloat, StrictInt]] = Field(default=None, description="//TODO")
     q: Optional[Union[StrictFloat, StrictInt]] = Field(default=None, description="//TODO")
     __properties: ClassVar[List[str]] = ["parametersType", "n", "p", "q"]
 
     model_config = {
         "populate_by_name": True,
```

### Comparing `spacestudio-satellite-client-1.0.8/spacestudio_satellite_client/models/comparison_item.py` & `spacestudio-satellite-client-1.0.9/spacestudio_satellite_client/models/comparison_item.py`

 * *Files identical despite different names*

### Comparing `spacestudio-satellite-client-1.0.8/spacestudio_satellite_client/models/comparison_item1.py` & `spacestudio-satellite-client-1.0.9/spacestudio_satellite_client/models/comparison_item1.py`

 * *Files identical despite different names*

### Comparing `spacestudio-satellite-client-1.0.8/spacestudio_satellite_client/models/computation.py` & `spacestudio-satellite-client-1.0.9/spacestudio_satellite_client/models/computation.py`

 * *Files identical despite different names*

### Comparing `spacestudio-satellite-client-1.0.8/spacestudio_satellite_client/models/computation_mode.py` & `spacestudio-satellite-client-1.0.9/spacestudio_satellite_client/models/computation_mode.py`

 * *Files identical despite different names*

### Comparing `spacestudio-satellite-client-1.0.8/spacestudio_satellite_client/models/computation_outputs.py` & `spacestudio-satellite-client-1.0.9/spacestudio_satellite_client/models/computation_outputs.py`

 * *Files 8% similar despite different names*

```diff
@@ -97,10 +97,12 @@
             klass = globals()[object_type]
             return klass.from_dict(obj)
         else:
             raise ValueError("ComputationOutputs failed to lookup discriminator value from " +
                              json.dumps(obj) + ". Discriminator property name: " + cls.__discriminator_property_name +
                              ", mapping: " + json.dumps(cls.__discriminator_value_class_map))
 
+from spacestudio_satellite_client.models.single_satellite_analytical_computation_outputs import SingleSatelliteAnalyticalComputationOutputs
+from spacestudio_satellite_client.models.single_satellite_numerical_computation_outputs import SingleSatelliteNumericalComputationOutputs
 # TODO: Rewrite to not use raise_errors
 ComputationOutputs.model_rebuild(raise_errors=False)
```

### Comparing `spacestudio-satellite-client-1.0.8/spacestudio_satellite_client/models/computation_status.py` & `spacestudio-satellite-client-1.0.9/spacestudio_satellite_client/models/computation_status.py`

 * *Files identical despite different names*

### Comparing `spacestudio-satellite-client-1.0.8/spacestudio_satellite_client/models/computation_type.py` & `spacestudio-satellite-client-1.0.9/spacestudio_satellite_client/models/computation_type.py`

 * *Files identical despite different names*

### Comparing `spacestudio-satellite-client-1.0.8/spacestudio_satellite_client/models/context_outputs.py` & `spacestudio-satellite-client-1.0.9/spacestudio_satellite_client/models/context_outputs.py`

 * *Files identical despite different names*

### Comparing `spacestudio-satellite-client-1.0.8/spacestudio_satellite_client/models/deorbitation.py` & `spacestudio-satellite-client-1.0.9/spacestudio_satellite_client/models/deorbitation.py`

 * *Files identical despite different names*

### Comparing `spacestudio-satellite-client-1.0.8/spacestudio_satellite_client/models/display_configuration.py` & `spacestudio-satellite-client-1.0.9/spacestudio_satellite_client/models/display_configuration.py`

 * *Files identical despite different names*

### Comparing `spacestudio-satellite-client-1.0.8/spacestudio_satellite_client/models/display_configuration_comparison_overview.py` & `spacestudio-satellite-client-1.0.9/spacestudio_satellite_client/models/display_configuration_comparison_overview.py`

 * *Files identical despite different names*

### Comparing `spacestudio-satellite-client-1.0.8/spacestudio_satellite_client/models/drag_perturbation.py` & `spacestudio-satellite-client-1.0.9/spacestudio_satellite_client/models/drag_perturbation.py`

 * *Files identical despite different names*

### Comparing `spacestudio-satellite-client-1.0.8/spacestudio_satellite_client/models/duplicate_scenario_request.py` & `spacestudio-satellite-client-1.0.9/spacestudio_satellite_client/models/duplicate_scenario_request.py`

 * *Files identical despite different names*

### Comparing `spacestudio-satellite-client-1.0.8/spacestudio_satellite_client/models/earth_potential_configuration.py` & `spacestudio-satellite-client-1.0.9/spacestudio_satellite_client/models/earth_potential_configuration.py`

 * *Files identical despite different names*

### Comparing `spacestudio-satellite-client-1.0.8/spacestudio_satellite_client/models/earth_potential_perturbation.py` & `spacestudio-satellite-client-1.0.9/spacestudio_satellite_client/models/earth_potential_perturbation.py`

 * *Files identical despite different names*

### Comparing `spacestudio-satellite-client-1.0.8/spacestudio_satellite_client/models/elliptical_ground_track_repeated_eccentricity_orbit_parameters.py` & `spacestudio-satellite-client-1.0.9/spacestudio_satellite_client/models/elliptical_ground_track_repeated_eccentricity_orbit_parameters.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,24 +13,24 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import Field, StrictFloat, StrictInt
+from pydantic import BaseModel, Field, StrictFloat, StrictInt, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional, Union
-from spacestudio_satellite_client.models.orbit_parameters import OrbitParameters
 from typing import Optional, Set
 from typing_extensions import Self
 
-class EllipticalGroundTrackRepeatedEccentricityOrbitParameters(OrbitParameters):
+class EllipticalGroundTrackRepeatedEccentricityOrbitParameters(BaseModel):
     """
     EllipticalGroundTrackRepeatedEccentricityOrbitParameters
     """ # noqa: E501
+    parameters_type: Optional[StrictStr] = Field(default=None, alias="parametersType")
     n: Optional[Union[StrictFloat, StrictInt]] = Field(default=None, description="//TODO")
     p: Optional[Union[StrictFloat, StrictInt]] = Field(default=None, description="//TODO")
     q: Optional[Union[StrictFloat, StrictInt]] = Field(default=None, description="//TODO")
     __properties: ClassVar[List[str]] = ["parametersType", "n", "p", "q"]
 
     model_config = {
         "populate_by_name": True,
```

### Comparing `spacestudio-satellite-client-1.0.8/spacestudio_satellite_client/models/elliptical_perigee_alt_apogee_alt_orbit_parameters.py` & `spacestudio-satellite-client-1.0.9/spacestudio_satellite_client/models/elliptical_perigee_alt_apogee_alt_orbit_parameters.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,24 +13,24 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import Field, StrictFloat, StrictInt
+from pydantic import BaseModel, Field, StrictFloat, StrictInt, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional, Union
-from spacestudio_satellite_client.models.orbit_parameters import OrbitParameters
 from typing import Optional, Set
 from typing_extensions import Self
 
-class EllipticalPerigeeAltApogeeAltOrbitParameters(OrbitParameters):
+class EllipticalPerigeeAltApogeeAltOrbitParameters(BaseModel):
     """
     EllipticalPerigeeAltApogeeAltOrbitParameters
     """ # noqa: E501
+    parameters_type: Optional[StrictStr] = Field(default=None, alias="parametersType")
     perigee_altitude: Optional[Union[StrictFloat, StrictInt]] = Field(default=None, description="The orbit perigee altitude (in meters)", alias="perigeeAltitude")
     apogee_altitude: Optional[Union[StrictFloat, StrictInt]] = Field(default=None, description="The orbit apogee altitude (in meters)", alias="apogeeAltitude")
     __properties: ClassVar[List[str]] = ["parametersType", "perigeeAltitude", "apogeeAltitude"]
 
     model_config = {
         "populate_by_name": True,
         "validate_assignment": True,
```

### Comparing `spacestudio-satellite-client-1.0.8/spacestudio_satellite_client/models/elliptical_perigee_alt_eccentricity_orbit_parameters.py` & `spacestudio-satellite-client-1.0.9/spacestudio_satellite_client/models/elliptical_perigee_alt_eccentricity_orbit_parameters.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,24 +13,24 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import Field, StrictFloat, StrictInt
+from pydantic import BaseModel, Field, StrictFloat, StrictInt, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional, Union
-from spacestudio_satellite_client.models.orbit_parameters import OrbitParameters
 from typing import Optional, Set
 from typing_extensions import Self
 
-class EllipticalPerigeeAltEccentricityOrbitParameters(OrbitParameters):
+class EllipticalPerigeeAltEccentricityOrbitParameters(BaseModel):
     """
     EllipticalPerigeeAltEccentricityOrbitParameters
     """ # noqa: E501
+    parameters_type: Optional[StrictStr] = Field(default=None, alias="parametersType")
     perigee_altitude: Optional[Union[StrictFloat, StrictInt]] = Field(default=None, description="The orbit perigee altitude (in meters)", alias="perigeeAltitude")
     __properties: ClassVar[List[str]] = ["parametersType", "perigeeAltitude"]
 
     model_config = {
         "populate_by_name": True,
         "validate_assignment": True,
         "protected_namespaces": (),
```

### Comparing `spacestudio-satellite-client-1.0.8/spacestudio_satellite_client/models/elliptical_sma_eccentricity_orbit_parameters.py` & `spacestudio-satellite-client-1.0.9/spacestudio_satellite_client/models/elliptical_sma_eccentricity_orbit_parameters.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,23 +13,24 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from typing import Any, ClassVar, Dict, List
-from spacestudio_satellite_client.models.orbit_parameters import OrbitParameters
+from pydantic import BaseModel, Field, StrictStr
+from typing import Any, ClassVar, Dict, List, Optional
 from typing import Optional, Set
 from typing_extensions import Self
 
-class EllipticalSmaEccentricityOrbitParameters(OrbitParameters):
+class EllipticalSmaEccentricityOrbitParameters(BaseModel):
     """
     EllipticalSmaEccentricityOrbitParameters
     """ # noqa: E501
+    parameters_type: Optional[StrictStr] = Field(default=None, alias="parametersType")
     __properties: ClassVar[List[str]] = ["parametersType"]
 
     model_config = {
         "populate_by_name": True,
         "validate_assignment": True,
         "protected_namespaces": (),
     }
```

### Comparing `spacestudio-satellite-client-1.0.8/spacestudio_satellite_client/models/leo_station_keeping.py` & `spacestudio-satellite-client-1.0.9/spacestudio_satellite_client/models/leo_station_keeping.py`

 * *Files identical despite different names*

### Comparing `spacestudio-satellite-client-1.0.8/spacestudio_satellite_client/models/maneuver.py` & `spacestudio-satellite-client-1.0.9/spacestudio_satellite_client/models/timeline_slot.py`

 * *Files 19% similar despite different names*

```diff
@@ -13,49 +13,61 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, StrictStr, field_validator
+from pydantic import BaseModel, Field, StrictStr, field_validator
 from typing import Any, ClassVar, Dict, List, Optional, Union
 from typing import Optional, Set
 from typing_extensions import Self
 
-class Maneuver(BaseModel):
+class TimelineSlot(BaseModel):
     """
-    Maneuver
+    TimelineSlot
     """ # noqa: E501
     type: Optional[StrictStr] = None
-    __properties: ClassVar[List[str]] = ["type"]
+    id: Optional[StrictStr] = Field(default=None, description="The unique identifier of the event")
+    validity: Optional[StrictStr] = Field(default=None, description="The validity of the event")
+    __properties: ClassVar[List[str]] = ["type", "id", "validity"]
 
     @field_validator('type')
     def type_validate_enum(cls, value):
         """Validates the enum"""
         if value is None:
             return value
 
-        if value not in set(['ORBITAL_TRANSFER', 'RAAN_PHASING', 'ORBIT_PHASING', 'LEO_STATION_KEEPING', 'DEORBITATION', 'ORBIT_PROPAGATION']):
-            raise ValueError("must be one of enum values ('ORBITAL_TRANSFER', 'RAAN_PHASING', 'ORBIT_PHASING', 'LEO_STATION_KEEPING', 'DEORBITATION', 'ORBIT_PROPAGATION')")
+        if value not in set(['ORBIT', 'MANEUVER']):
+            raise ValueError("must be one of enum values ('ORBIT', 'MANEUVER')")
+        return value
+
+    @field_validator('validity')
+    def validity_validate_enum(cls, value):
+        """Validates the enum"""
+        if value is None:
+            return value
+
+        if value not in set(['VALID', 'INVALID']):
+            raise ValueError("must be one of enum values ('VALID', 'INVALID')")
         return value
 
     model_config = {
         "populate_by_name": True,
         "validate_assignment": True,
         "protected_namespaces": (),
     }
 
 
     # JSON field name that stores the object type
     __discriminator_property_name: ClassVar[str] = 'type'
 
     # discriminator mappings
     __discriminator_value_class_map: ClassVar[Dict[str, str]] = {
-        'DEORBITATION': 'Deorbitation','LEO_STATION_KEEPING': 'LeoStationKeeping','ORBITAL_TRANSFER': 'OrbitalTransfer','ORBIT_PHASING': 'OrbitPhasing','ORBIT_PROPAGATION': 'OrbitPropagation','RAAN_PHASING': 'RaanPhasing'
+        'MANEUVER': 'ManeuverTimelineSlot','ORBIT': 'OrbitTimelineSlot'
     }
 
     @classmethod
     def get_discriminator_value(cls, obj: Dict[str, Any]) -> Optional[str]:
         """Returns the discriminator value (object type) of the data"""
         discriminator_value = obj[cls.__discriminator_property_name]
         if discriminator_value:
@@ -69,16 +81,16 @@
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> Optional[Union[Self, Self, Self, Self, Self, Self]]:
-        """Create an instance of Maneuver from a JSON string"""
+    def from_json(cls, json_str: str) -> Optional[Union[Self, Self]]:
+        """Create an instance of TimelineSlot from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -94,22 +106,24 @@
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: Dict[str, Any]) -> Optional[Union[Self, Self, Self, Self, Self, Self]]:
-        """Create an instance of Maneuver from a dict"""
+    def from_dict(cls, obj: Dict[str, Any]) -> Optional[Union[Self, Self]]:
+        """Create an instance of TimelineSlot from a dict"""
         # look up the object type based on discriminator mapping
         object_type = cls.get_discriminator_value(obj)
         if object_type:
             klass = globals()[object_type]
             return klass.from_dict(obj)
         else:
-            raise ValueError("Maneuver failed to lookup discriminator value from " +
+            raise ValueError("TimelineSlot failed to lookup discriminator value from " +
                              json.dumps(obj) + ". Discriminator property name: " + cls.__discriminator_property_name +
                              ", mapping: " + json.dumps(cls.__discriminator_value_class_map))
 
+from spacestudio_satellite_client.models.maneuver_timeline_slot import ManeuverTimelineSlot
+from spacestudio_satellite_client.models.orbit_timeline_slot import OrbitTimelineSlot
 # TODO: Rewrite to not use raise_errors
-Maneuver.model_rebuild(raise_errors=False)
+TimelineSlot.model_rebuild(raise_errors=False)
```

### Comparing `spacestudio-satellite-client-1.0.8/spacestudio_satellite_client/models/maneuver_timeline_slot.py` & `spacestudio-satellite-client-1.0.9/spacestudio_satellite_client/models/maneuver_timeline_slot.py`

 * *Files identical despite different names*

### Comparing `spacestudio-satellite-client-1.0.8/spacestudio_satellite_client/models/maneuvering_strategy.py` & `spacestudio-satellite-client-1.0.9/spacestudio_satellite_client/models/maneuvering_strategy.py`

 * *Files identical despite different names*

### Comparing `spacestudio-satellite-client-1.0.8/spacestudio_satellite_client/models/notification.py` & `spacestudio-satellite-client-1.0.9/spacestudio_satellite_client/models/notification.py`

 * *Files identical despite different names*

### Comparing `spacestudio-satellite-client-1.0.8/spacestudio_satellite_client/models/notification_content.py` & `spacestudio-satellite-client-1.0.9/spacestudio_satellite_client/models/notification_content.py`

 * *Files identical despite different names*

### Comparing `spacestudio-satellite-client-1.0.8/spacestudio_satellite_client/models/numerical_ephemeris.py` & `spacestudio-satellite-client-1.0.9/spacestudio_satellite_client/models/numerical_ephemeris.py`

 * *Files identical despite different names*

### Comparing `spacestudio-satellite-client-1.0.8/spacestudio_satellite_client/models/numerical_outputs_configuration.py` & `spacestudio-satellite-client-1.0.9/spacestudio_satellite_client/models/numerical_outputs_configuration.py`

 * *Files identical despite different names*

### Comparing `spacestudio-satellite-client-1.0.8/spacestudio_satellite_client/models/numerical_study_parameters.py` & `spacestudio-satellite-client-1.0.9/spacestudio_satellite_client/models/numerical_study_parameters.py`

 * *Files identical despite different names*

### Comparing `spacestudio-satellite-client-1.0.8/spacestudio_satellite_client/models/orbit.py` & `spacestudio-satellite-client-1.0.9/spacestudio_satellite_client/models/orbit.py`

 * *Files identical despite different names*

### Comparing `spacestudio-satellite-client-1.0.8/spacestudio_satellite_client/models/orbit_parameters.py` & `spacestudio-satellite-client-1.0.9/spacestudio_satellite_client/models/study_parameters.py`

 * *Files 20% similar despite different names*

```diff
@@ -13,49 +13,44 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, Field, StrictStr, field_validator
+from pydantic import BaseModel, Field
 from typing import Any, ClassVar, Dict, List, Optional, Union
+from spacestudio_satellite_client.models.computation_mode import ComputationMode
+from spacestudio_satellite_client.models.context_outputs import ContextOutputs
+from spacestudio_satellite_client.models.maneuver import Maneuver
 from typing import Optional, Set
 from typing_extensions import Self
 
-class OrbitParameters(BaseModel):
+class StudyParameters(BaseModel):
     """
-    The orbit parameters
+    StudyParameters
     """ # noqa: E501
-    parameters_type: Optional[StrictStr] = Field(default=None, description="The orbit parameters type", alias="parametersType")
-    __properties: ClassVar[List[str]] = ["parametersType"]
-
-    @field_validator('parameters_type')
-    def parameters_type_validate_enum(cls, value):
-        """Validates the enum"""
-        if value is None:
-            return value
-
-        if value not in set(['CIRCULAR_ALTITUDE', 'CIRCULAR_GROUND_TRACK_REPEATED', 'ELLIPTICAL_PERIGEE_ALTITUDE_ECC', 'ELLIPTICAL_GROUND_TRACK_REPEATED_ECC', 'ELLIPTICAL_PERIGEE_ALTITUDE_APOGEE_ALTITUDE', 'ELLIPTICAL_SMA_ECC']):
-            raise ValueError("must be one of enum values ('CIRCULAR_ALTITUDE', 'CIRCULAR_GROUND_TRACK_REPEATED', 'ELLIPTICAL_PERIGEE_ALTITUDE_ECC', 'ELLIPTICAL_GROUND_TRACK_REPEATED_ECC', 'ELLIPTICAL_PERIGEE_ALTITUDE_APOGEE_ALTITUDE', 'ELLIPTICAL_SMA_ECC')")
-        return value
+    computation_mode: Optional[ComputationMode] = Field(default=None, alias="computationMode")
+    maneuver: Optional[Maneuver] = None
+    context_outputs: Optional[ContextOutputs] = Field(default=None, alias="contextOutputs")
+    __properties: ClassVar[List[str]] = ["computationMode", "maneuver", "contextOutputs"]
 
     model_config = {
         "populate_by_name": True,
         "validate_assignment": True,
         "protected_namespaces": (),
     }
 
 
     # JSON field name that stores the object type
-    __discriminator_property_name: ClassVar[str] = 'parametersType'
+    __discriminator_property_name: ClassVar[str] = 'computationMode'
 
     # discriminator mappings
     __discriminator_value_class_map: ClassVar[Dict[str, str]] = {
-        'CIRCULAR_ALTITUDE': 'CircularAltitudeOrbitParameters','CIRCULAR_GROUND_TRACK_REPEATED': 'CircularGroundTrackRepeatedOrbitParameters','ELLIPTICAL_GROUND_TRACK_REPEATED_ECC': 'EllipticalGroundTrackRepeatedEccentricityOrbitParameters','ELLIPTICAL_PERIGEE_ALTITUDE_APOGEE_ALTITUDE': 'EllipticalPerigeeAltApogeeAltOrbitParameters','ELLIPTICAL_PERIGEE_ALTITUDE_ECC': 'EllipticalPerigeeAltEccentricityOrbitParameters','ELLIPTICAL_SMA_ECC': 'EllipticalSmaEccentricityOrbitParameters'
+        'ANALYTICAL': 'AnalyticalStudyParameters','NUMERICAL': 'NumericalStudyParameters'
     }
 
     @classmethod
     def get_discriminator_value(cls, obj: Dict[str, Any]) -> Optional[str]:
         """Returns the discriminator value (object type) of the data"""
         discriminator_value = obj[cls.__discriminator_property_name]
         if discriminator_value:
@@ -69,16 +64,16 @@
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> Optional[Union[Self, Self, Self, Self, Self, Self]]:
-        """Create an instance of OrbitParameters from a JSON string"""
+    def from_json(cls, json_str: str) -> Optional[Union[Self, Self]]:
+        """Create an instance of StudyParameters from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -91,25 +86,33 @@
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
+        # override the default output from pydantic by calling `to_dict()` of maneuver
+        if self.maneuver:
+            _dict['maneuver'] = self.maneuver.to_dict()
+        # override the default output from pydantic by calling `to_dict()` of context_outputs
+        if self.context_outputs:
+            _dict['contextOutputs'] = self.context_outputs.to_dict()
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: Dict[str, Any]) -> Optional[Union[Self, Self, Self, Self, Self, Self]]:
-        """Create an instance of OrbitParameters from a dict"""
+    def from_dict(cls, obj: Dict[str, Any]) -> Optional[Union[Self, Self]]:
+        """Create an instance of StudyParameters from a dict"""
         # look up the object type based on discriminator mapping
         object_type = cls.get_discriminator_value(obj)
         if object_type:
             klass = globals()[object_type]
             return klass.from_dict(obj)
         else:
-            raise ValueError("OrbitParameters failed to lookup discriminator value from " +
+            raise ValueError("StudyParameters failed to lookup discriminator value from " +
                              json.dumps(obj) + ". Discriminator property name: " + cls.__discriminator_property_name +
                              ", mapping: " + json.dumps(cls.__discriminator_value_class_map))
 
+from spacestudio_satellite_client.models.analytical_study_parameters import AnalyticalStudyParameters
+from spacestudio_satellite_client.models.numerical_study_parameters import NumericalStudyParameters
 # TODO: Rewrite to not use raise_errors
-OrbitParameters.model_rebuild(raise_errors=False)
+StudyParameters.model_rebuild(raise_errors=False)
```

### Comparing `spacestudio-satellite-client-1.0.8/spacestudio_satellite_client/models/orbit_phasing.py` & `spacestudio-satellite-client-1.0.9/spacestudio_satellite_client/models/orbit_phasing.py`

 * *Files identical despite different names*

### Comparing `spacestudio-satellite-client-1.0.8/spacestudio_satellite_client/models/orbit_propagation.py` & `spacestudio-satellite-client-1.0.9/spacestudio_satellite_client/models/orbit_propagation.py`

 * *Files identical despite different names*

### Comparing `spacestudio-satellite-client-1.0.8/spacestudio_satellite_client/models/orbit_timeline_slot.py` & `spacestudio-satellite-client-1.0.9/spacestudio_satellite_client/models/orbit_timeline_slot.py`

 * *Files identical despite different names*

### Comparing `spacestudio-satellite-client-1.0.8/spacestudio_satellite_client/models/orbital_transfer.py` & `spacestudio-satellite-client-1.0.9/spacestudio_satellite_client/models/orbital_transfer.py`

 * *Files identical despite different names*

### Comparing `spacestudio-satellite-client-1.0.8/spacestudio_satellite_client/models/payload.py` & `spacestudio-satellite-client-1.0.9/spacestudio_satellite_client/models/payload.py`

 * *Files identical despite different names*

### Comparing `spacestudio-satellite-client-1.0.8/spacestudio_satellite_client/models/perturbation.py` & `spacestudio-satellite-client-1.0.9/spacestudio_satellite_client/models/perturbation.py`

 * *Files 20% similar despite different names*

```diff
@@ -97,10 +97,14 @@
             klass = globals()[object_type]
             return klass.from_dict(obj)
         else:
             raise ValueError("Perturbation failed to lookup discriminator value from " +
                              json.dumps(obj) + ". Discriminator property name: " + cls.__discriminator_property_name +
                              ", mapping: " + json.dumps(cls.__discriminator_value_class_map))
 
+from spacestudio_satellite_client.models.drag_perturbation import DragPerturbation
+from spacestudio_satellite_client.models.earth_potential_perturbation import EarthPotentialPerturbation
+from spacestudio_satellite_client.models.solar_radiation_pressure_perturbation import SolarRadiationPressurePerturbation
+from spacestudio_satellite_client.models.third_body_perturbation import ThirdBodyPerturbation
 # TODO: Rewrite to not use raise_errors
 Perturbation.model_rebuild(raise_errors=False)
```

### Comparing `spacestudio-satellite-client-1.0.8/spacestudio_satellite_client/models/perturbation_type.py` & `spacestudio-satellite-client-1.0.9/spacestudio_satellite_client/models/perturbation_type.py`

 * *Files identical despite different names*

### Comparing `spacestudio-satellite-client-1.0.8/spacestudio_satellite_client/models/platform.py` & `spacestudio-satellite-client-1.0.9/spacestudio_satellite_client/models/platform.py`

 * *Files identical despite different names*

### Comparing `spacestudio-satellite-client-1.0.8/spacestudio_satellite_client/models/plot.py` & `spacestudio-satellite-client-1.0.9/spacestudio_satellite_client/models/plot.py`

 * *Files identical despite different names*

### Comparing `spacestudio-satellite-client-1.0.8/spacestudio_satellite_client/models/propulsion_system.py` & `spacestudio-satellite-client-1.0.9/spacestudio_satellite_client/models/propulsion_system.py`

 * *Files identical despite different names*

### Comparing `spacestudio-satellite-client-1.0.8/spacestudio_satellite_client/models/raan_phasing.py` & `spacestudio-satellite-client-1.0.9/spacestudio_satellite_client/models/raan_phasing.py`

 * *Files identical despite different names*

### Comparing `spacestudio-satellite-client-1.0.8/spacestudio_satellite_client/models/scenario.py` & `spacestudio-satellite-client-1.0.9/spacestudio_satellite_client/models/scenario.py`

 * *Files identical despite different names*

### Comparing `spacestudio-satellite-client-1.0.8/spacestudio_satellite_client/models/scenario_baseline.py` & `spacestudio-satellite-client-1.0.9/spacestudio_satellite_client/models/scenario_baseline.py`

 * *Files identical despite different names*

### Comparing `spacestudio-satellite-client-1.0.8/spacestudio_satellite_client/models/simulation_configuration.py` & `spacestudio-satellite-client-1.0.9/spacestudio_satellite_client/models/simulation_configuration.py`

 * *Files identical despite different names*

### Comparing `spacestudio-satellite-client-1.0.8/spacestudio_satellite_client/models/single_satellite_analytical_computation_outputs.py` & `spacestudio-satellite-client-1.0.9/spacestudio_satellite_client/models/single_satellite_analytical_computation_outputs.py`

 * *Files identical despite different names*

### Comparing `spacestudio-satellite-client-1.0.8/spacestudio_satellite_client/models/single_satellite_numerical_computation_outputs.py` & `spacestudio-satellite-client-1.0.9/spacestudio_satellite_client/models/single_satellite_numerical_computation_outputs.py`

 * *Files identical despite different names*

### Comparing `spacestudio-satellite-client-1.0.8/spacestudio_satellite_client/models/solar_radiation_pressure_perturbation.py` & `spacestudio-satellite-client-1.0.9/spacestudio_satellite_client/models/solar_radiation_pressure_perturbation.py`

 * *Files identical despite different names*

### Comparing `spacestudio-satellite-client-1.0.8/spacestudio_satellite_client/models/spacecraft_geometry.py` & `spacestudio-satellite-client-1.0.9/spacestudio_satellite_client/models/spacecraft_geometry.py`

 * *Files identical despite different names*

### Comparing `spacestudio-satellite-client-1.0.8/spacestudio_satellite_client/models/study.py` & `spacestudio-satellite-client-1.0.9/spacestudio_satellite_client/models/study.py`

 * *Files identical despite different names*

### Comparing `spacestudio-satellite-client-1.0.8/spacestudio_satellite_client/models/study_computation.py` & `spacestudio-satellite-client-1.0.9/spacestudio_satellite_client/models/study_computation.py`

 * *Files identical despite different names*

### Comparing `spacestudio-satellite-client-1.0.8/spacestudio_satellite_client/models/study_inputs.py` & `spacestudio-satellite-client-1.0.9/spacestudio_satellite_client/models/study_inputs.py`

 * *Files identical despite different names*

### Comparing `spacestudio-satellite-client-1.0.8/spacestudio_satellite_client/models/study_parameters.py` & `spacestudio-satellite-client-1.0.9/spacestudio_satellite_client/models/maneuver.py`

 * *Files 24% similar despite different names*

```diff
@@ -13,44 +13,49 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, Field
+from pydantic import BaseModel, StrictStr, field_validator
 from typing import Any, ClassVar, Dict, List, Optional, Union
-from spacestudio_satellite_client.models.computation_mode import ComputationMode
-from spacestudio_satellite_client.models.context_outputs import ContextOutputs
-from spacestudio_satellite_client.models.maneuver import Maneuver
 from typing import Optional, Set
 from typing_extensions import Self
 
-class StudyParameters(BaseModel):
+class Maneuver(BaseModel):
     """
-    StudyParameters
+    Maneuver
     """ # noqa: E501
-    computation_mode: Optional[ComputationMode] = Field(default=None, alias="computationMode")
-    maneuver: Optional[Maneuver] = None
-    context_outputs: Optional[ContextOutputs] = Field(default=None, alias="contextOutputs")
-    __properties: ClassVar[List[str]] = ["computationMode", "maneuver", "contextOutputs"]
+    type: Optional[StrictStr] = None
+    __properties: ClassVar[List[str]] = ["type"]
+
+    @field_validator('type')
+    def type_validate_enum(cls, value):
+        """Validates the enum"""
+        if value is None:
+            return value
+
+        if value not in set(['ORBITAL_TRANSFER', 'RAAN_PHASING', 'ORBIT_PHASING', 'LEO_STATION_KEEPING', 'DEORBITATION', 'ORBIT_PROPAGATION']):
+            raise ValueError("must be one of enum values ('ORBITAL_TRANSFER', 'RAAN_PHASING', 'ORBIT_PHASING', 'LEO_STATION_KEEPING', 'DEORBITATION', 'ORBIT_PROPAGATION')")
+        return value
 
     model_config = {
         "populate_by_name": True,
         "validate_assignment": True,
         "protected_namespaces": (),
     }
 
 
     # JSON field name that stores the object type
-    __discriminator_property_name: ClassVar[str] = 'computationMode'
+    __discriminator_property_name: ClassVar[str] = 'type'
 
     # discriminator mappings
     __discriminator_value_class_map: ClassVar[Dict[str, str]] = {
-        'ANALYTICAL': 'AnalyticalStudyParameters','NUMERICAL': 'NumericalStudyParameters'
+        'DEORBITATION': 'Deorbitation','LEO_STATION_KEEPING': 'LeoStationKeeping','ORBITAL_TRANSFER': 'OrbitalTransfer','ORBIT_PHASING': 'OrbitPhasing','ORBIT_PROPAGATION': 'OrbitPropagation','RAAN_PHASING': 'RaanPhasing'
     }
 
     @classmethod
     def get_discriminator_value(cls, obj: Dict[str, Any]) -> Optional[str]:
         """Returns the discriminator value (object type) of the data"""
         discriminator_value = obj[cls.__discriminator_property_name]
         if discriminator_value:
@@ -64,16 +69,16 @@
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> Optional[Union[Self, Self]]:
-        """Create an instance of StudyParameters from a JSON string"""
+    def from_json(cls, json_str: str) -> Optional[Union[Self, Self, Self, Self, Self, Self]]:
+        """Create an instance of Maneuver from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -86,31 +91,31 @@
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
-        # override the default output from pydantic by calling `to_dict()` of maneuver
-        if self.maneuver:
-            _dict['maneuver'] = self.maneuver.to_dict()
-        # override the default output from pydantic by calling `to_dict()` of context_outputs
-        if self.context_outputs:
-            _dict['contextOutputs'] = self.context_outputs.to_dict()
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: Dict[str, Any]) -> Optional[Union[Self, Self]]:
-        """Create an instance of StudyParameters from a dict"""
+    def from_dict(cls, obj: Dict[str, Any]) -> Optional[Union[Self, Self, Self, Self, Self, Self]]:
+        """Create an instance of Maneuver from a dict"""
         # look up the object type based on discriminator mapping
         object_type = cls.get_discriminator_value(obj)
         if object_type:
             klass = globals()[object_type]
             return klass.from_dict(obj)
         else:
-            raise ValueError("StudyParameters failed to lookup discriminator value from " +
+            raise ValueError("Maneuver failed to lookup discriminator value from " +
                              json.dumps(obj) + ". Discriminator property name: " + cls.__discriminator_property_name +
                              ", mapping: " + json.dumps(cls.__discriminator_value_class_map))
 
+from spacestudio_satellite_client.models.deorbitation import Deorbitation
+from spacestudio_satellite_client.models.leo_station_keeping import LeoStationKeeping
+from spacestudio_satellite_client.models.orbit_phasing import OrbitPhasing
+from spacestudio_satellite_client.models.orbit_propagation import OrbitPropagation
+from spacestudio_satellite_client.models.orbital_transfer import OrbitalTransfer
+from spacestudio_satellite_client.models.raan_phasing import RaanPhasing
 # TODO: Rewrite to not use raise_errors
-StudyParameters.model_rebuild(raise_errors=False)
+Maneuver.model_rebuild(raise_errors=False)
```

### Comparing `spacestudio-satellite-client-1.0.8/spacestudio_satellite_client/models/tab.py` & `spacestudio-satellite-client-1.0.9/spacestudio_satellite_client/models/tab.py`

 * *Files identical despite different names*

### Comparing `spacestudio-satellite-client-1.0.8/spacestudio_satellite_client/models/third_body_perturbation.py` & `spacestudio-satellite-client-1.0.9/spacestudio_satellite_client/models/third_body_perturbation.py`

 * *Files identical despite different names*

### Comparing `spacestudio-satellite-client-1.0.8/spacestudio_satellite_client/models/thrust_arcs_position.py` & `spacestudio-satellite-client-1.0.9/spacestudio_satellite_client/models/thrust_arcs_position.py`

 * *Files identical despite different names*

### Comparing `spacestudio-satellite-client-1.0.8/spacestudio_satellite_client/rest.py` & `spacestudio-satellite-client-1.0.9/spacestudio_satellite_client/rest.py`

 * *Files identical despite different names*

### Comparing `spacestudio-satellite-client-1.0.8/spacestudio_satellite_client.egg-info/PKG-INFO` & `spacestudio-satellite-client-1.0.9/spacestudio_satellite_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spacestudio-satellite-client
-Version: 1.0.8
+Version: 1.0.9
 Summary: Spacestudio API documentation
 Home-page: 
 Author: OpenAPI Generator community
 Author-email: team@openapitools.org
 Keywords: OpenAPI,OpenAPI-Generator,Spacestudio API documentation
 Description-Content-Type: text/markdown
 Requires-Dist: urllib3<2.1.0,>=1.25.3
```

### Comparing `spacestudio-satellite-client-1.0.8/spacestudio_satellite_client.egg-info/SOURCES.txt` & `spacestudio-satellite-client-1.0.9/spacestudio_satellite_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `spacestudio-satellite-client-1.0.8/test/test_advanced_orbit_parameters.py` & `spacestudio-satellite-client-1.0.9/test/test_advanced_orbit_parameters.py`

 * *Files identical despite different names*

### Comparing `spacestudio-satellite-client-1.0.8/test/test_analytical_study_parameters.py` & `spacestudio-satellite-client-1.0.9/test/test_analytical_study_parameters.py`

 * *Files identical despite different names*

### Comparing `spacestudio-satellite-client-1.0.8/test/test_announcement.py` & `spacestudio-satellite-client-1.0.9/test/test_announcement.py`

 * *Files identical despite different names*

### Comparing `spacestudio-satellite-client-1.0.8/test/test_announcement_api.py` & `spacestudio-satellite-client-1.0.9/test/test_announcement_api.py`

 * *Files identical despite different names*

### Comparing `spacestudio-satellite-client-1.0.8/test/test_baseline_configuration.py` & `spacestudio-satellite-client-1.0.9/test/test_baseline_configuration.py`

 * *Files identical despite different names*

### Comparing `spacestudio-satellite-client-1.0.8/test/test_circular_altitude_orbit_parameters.py` & `spacestudio-satellite-client-1.0.9/test/test_circular_altitude_orbit_parameters.py`

 * *Files identical despite different names*

### Comparing `spacestudio-satellite-client-1.0.8/test/test_circular_ground_track_repeated_orbit_parameters.py` & `spacestudio-satellite-client-1.0.9/test/test_circular_ground_track_repeated_orbit_parameters.py`

 * *Files identical despite different names*

### Comparing `spacestudio-satellite-client-1.0.8/test/test_comparison_item.py` & `spacestudio-satellite-client-1.0.9/test/test_comparison_item.py`

 * *Files identical despite different names*

### Comparing `spacestudio-satellite-client-1.0.8/test/test_comparison_item1.py` & `spacestudio-satellite-client-1.0.9/test/test_comparison_item1.py`

 * *Files identical despite different names*

### Comparing `spacestudio-satellite-client-1.0.8/test/test_computation.py` & `spacestudio-satellite-client-1.0.9/test/test_computation.py`

 * *Files identical despite different names*

### Comparing `spacestudio-satellite-client-1.0.8/test/test_computation_mode.py` & `spacestudio-satellite-client-1.0.9/test/test_computation_mode.py`

 * *Files identical despite different names*

### Comparing `spacestudio-satellite-client-1.0.8/test/test_computation_outputs.py` & `spacestudio-satellite-client-1.0.9/test/test_computation_outputs.py`

 * *Files identical despite different names*

### Comparing `spacestudio-satellite-client-1.0.8/test/test_computation_status.py` & `spacestudio-satellite-client-1.0.9/test/test_computation_status.py`

 * *Files identical despite different names*

### Comparing `spacestudio-satellite-client-1.0.8/test/test_computation_type.py` & `spacestudio-satellite-client-1.0.9/test/test_computation_type.py`

 * *Files identical despite different names*

### Comparing `spacestudio-satellite-client-1.0.8/test/test_computations_api.py` & `spacestudio-satellite-client-1.0.9/test/test_computations_api.py`

 * *Files identical despite different names*

### Comparing `spacestudio-satellite-client-1.0.8/test/test_context_outputs.py` & `spacestudio-satellite-client-1.0.9/test/test_context_outputs.py`

 * *Files identical despite different names*

### Comparing `spacestudio-satellite-client-1.0.8/test/test_deorbitation.py` & `spacestudio-satellite-client-1.0.9/test/test_deorbitation.py`

 * *Files identical despite different names*

### Comparing `spacestudio-satellite-client-1.0.8/test/test_display_configuration.py` & `spacestudio-satellite-client-1.0.9/test/test_display_configuration.py`

 * *Files identical despite different names*

### Comparing `spacestudio-satellite-client-1.0.8/test/test_display_configuration_comparison_overview.py` & `spacestudio-satellite-client-1.0.9/test/test_display_configuration_comparison_overview.py`

 * *Files identical despite different names*

### Comparing `spacestudio-satellite-client-1.0.8/test/test_drag_perturbation.py` & `spacestudio-satellite-client-1.0.9/test/test_drag_perturbation.py`

 * *Files identical despite different names*

### Comparing `spacestudio-satellite-client-1.0.8/test/test_duplicate_scenario_request.py` & `spacestudio-satellite-client-1.0.9/test/test_duplicate_scenario_request.py`

 * *Files identical despite different names*

### Comparing `spacestudio-satellite-client-1.0.8/test/test_earth_potential_configuration.py` & `spacestudio-satellite-client-1.0.9/test/test_earth_potential_configuration.py`

 * *Files identical despite different names*

### Comparing `spacestudio-satellite-client-1.0.8/test/test_earth_potential_perturbation.py` & `spacestudio-satellite-client-1.0.9/test/test_earth_potential_perturbation.py`

 * *Files identical despite different names*

### Comparing `spacestudio-satellite-client-1.0.8/test/test_elliptical_ground_track_repeated_eccentricity_orbit_parameters.py` & `spacestudio-satellite-client-1.0.9/test/test_elliptical_ground_track_repeated_eccentricity_orbit_parameters.py`

 * *Files identical despite different names*

### Comparing `spacestudio-satellite-client-1.0.8/test/test_elliptical_perigee_alt_apogee_alt_orbit_parameters.py` & `spacestudio-satellite-client-1.0.9/test/test_elliptical_perigee_alt_apogee_alt_orbit_parameters.py`

 * *Files identical despite different names*

### Comparing `spacestudio-satellite-client-1.0.8/test/test_elliptical_perigee_alt_eccentricity_orbit_parameters.py` & `spacestudio-satellite-client-1.0.9/test/test_elliptical_perigee_alt_eccentricity_orbit_parameters.py`

 * *Files identical despite different names*

### Comparing `spacestudio-satellite-client-1.0.8/test/test_elliptical_sma_eccentricity_orbit_parameters.py` & `spacestudio-satellite-client-1.0.9/test/test_elliptical_sma_eccentricity_orbit_parameters.py`

 * *Files identical despite different names*

### Comparing `spacestudio-satellite-client-1.0.8/test/test_leo_station_keeping.py` & `spacestudio-satellite-client-1.0.9/test/test_leo_station_keeping.py`

 * *Files identical despite different names*

### Comparing `spacestudio-satellite-client-1.0.8/test/test_maneuver.py` & `spacestudio-satellite-client-1.0.9/test/test_maneuver.py`

 * *Files identical despite different names*

### Comparing `spacestudio-satellite-client-1.0.8/test/test_maneuver_timeline_slot.py` & `spacestudio-satellite-client-1.0.9/test/test_maneuver_timeline_slot.py`

 * *Files identical despite different names*

### Comparing `spacestudio-satellite-client-1.0.8/test/test_maneuvering_strategy.py` & `spacestudio-satellite-client-1.0.9/test/test_maneuvering_strategy.py`

 * *Files identical despite different names*

### Comparing `spacestudio-satellite-client-1.0.8/test/test_notification.py` & `spacestudio-satellite-client-1.0.9/test/test_notification.py`

 * *Files identical despite different names*

### Comparing `spacestudio-satellite-client-1.0.8/test/test_notification_api.py` & `spacestudio-satellite-client-1.0.9/test/test_notification_api.py`

 * *Files identical despite different names*

### Comparing `spacestudio-satellite-client-1.0.8/test/test_notification_content.py` & `spacestudio-satellite-client-1.0.9/test/test_notification_content.py`

 * *Files identical despite different names*

### Comparing `spacestudio-satellite-client-1.0.8/test/test_numerical_ephemeris.py` & `spacestudio-satellite-client-1.0.9/test/test_numerical_ephemeris.py`

 * *Files identical despite different names*

### Comparing `spacestudio-satellite-client-1.0.8/test/test_numerical_outputs_configuration.py` & `spacestudio-satellite-client-1.0.9/test/test_numerical_outputs_configuration.py`

 * *Files identical despite different names*

### Comparing `spacestudio-satellite-client-1.0.8/test/test_numerical_study_parameters.py` & `spacestudio-satellite-client-1.0.9/test/test_numerical_study_parameters.py`

 * *Files identical despite different names*

### Comparing `spacestudio-satellite-client-1.0.8/test/test_orbit.py` & `spacestudio-satellite-client-1.0.9/test/test_orbit.py`

 * *Files identical despite different names*

### Comparing `spacestudio-satellite-client-1.0.8/test/test_orbit_parameters.py` & `spacestudio-satellite-client-1.0.9/test/test_orbit_parameters.py`

 * *Files identical despite different names*

### Comparing `spacestudio-satellite-client-1.0.8/test/test_orbit_phasing.py` & `spacestudio-satellite-client-1.0.9/test/test_orbit_phasing.py`

 * *Files identical despite different names*

### Comparing `spacestudio-satellite-client-1.0.8/test/test_orbit_propagation.py` & `spacestudio-satellite-client-1.0.9/test/test_orbit_propagation.py`

 * *Files identical despite different names*

### Comparing `spacestudio-satellite-client-1.0.8/test/test_orbit_timeline_slot.py` & `spacestudio-satellite-client-1.0.9/test/test_orbit_timeline_slot.py`

 * *Files identical despite different names*

### Comparing `spacestudio-satellite-client-1.0.8/test/test_orbital_transfer.py` & `spacestudio-satellite-client-1.0.9/test/test_orbital_transfer.py`

 * *Files identical despite different names*

### Comparing `spacestudio-satellite-client-1.0.8/test/test_orbits_api.py` & `spacestudio-satellite-client-1.0.9/test/test_orbits_api.py`

 * *Files identical despite different names*

### Comparing `spacestudio-satellite-client-1.0.8/test/test_payload.py` & `spacestudio-satellite-client-1.0.9/test/test_payload.py`

 * *Files identical despite different names*

### Comparing `spacestudio-satellite-client-1.0.8/test/test_perturbation.py` & `spacestudio-satellite-client-1.0.9/test/test_perturbation.py`

 * *Files identical despite different names*

### Comparing `spacestudio-satellite-client-1.0.8/test/test_perturbation_type.py` & `spacestudio-satellite-client-1.0.9/test/test_perturbation_type.py`

 * *Files identical despite different names*

### Comparing `spacestudio-satellite-client-1.0.8/test/test_platform.py` & `spacestudio-satellite-client-1.0.9/test/test_platform.py`

 * *Files identical despite different names*

### Comparing `spacestudio-satellite-client-1.0.8/test/test_platforms_api.py` & `spacestudio-satellite-client-1.0.9/test/test_platforms_api.py`

 * *Files identical despite different names*

### Comparing `spacestudio-satellite-client-1.0.8/test/test_plot.py` & `spacestudio-satellite-client-1.0.9/test/test_plot.py`

 * *Files identical despite different names*

### Comparing `spacestudio-satellite-client-1.0.8/test/test_propulsion_system.py` & `spacestudio-satellite-client-1.0.9/test/test_propulsion_system.py`

 * *Files identical despite different names*

### Comparing `spacestudio-satellite-client-1.0.8/test/test_propulsion_systems_api.py` & `spacestudio-satellite-client-1.0.9/test/test_propulsion_systems_api.py`

 * *Files identical despite different names*

### Comparing `spacestudio-satellite-client-1.0.8/test/test_raan_phasing.py` & `spacestudio-satellite-client-1.0.9/test/test_raan_phasing.py`

 * *Files identical despite different names*

### Comparing `spacestudio-satellite-client-1.0.8/test/test_scenario.py` & `spacestudio-satellite-client-1.0.9/test/test_scenario.py`

 * *Files identical despite different names*

### Comparing `spacestudio-satellite-client-1.0.8/test/test_scenario_baseline.py` & `spacestudio-satellite-client-1.0.9/test/test_scenario_baseline.py`

 * *Files identical despite different names*

### Comparing `spacestudio-satellite-client-1.0.8/test/test_scenarios_api.py` & `spacestudio-satellite-client-1.0.9/test/test_scenarios_api.py`

 * *Files identical despite different names*

### Comparing `spacestudio-satellite-client-1.0.8/test/test_simulation_configuration.py` & `spacestudio-satellite-client-1.0.9/test/test_simulation_configuration.py`

 * *Files identical despite different names*

### Comparing `spacestudio-satellite-client-1.0.8/test/test_single_satellite_analytical_computation_outputs.py` & `spacestudio-satellite-client-1.0.9/test/test_single_satellite_analytical_computation_outputs.py`

 * *Files identical despite different names*

### Comparing `spacestudio-satellite-client-1.0.8/test/test_single_satellite_numerical_computation_outputs.py` & `spacestudio-satellite-client-1.0.9/test/test_single_satellite_numerical_computation_outputs.py`

 * *Files identical despite different names*

### Comparing `spacestudio-satellite-client-1.0.8/test/test_solar_radiation_pressure_perturbation.py` & `spacestudio-satellite-client-1.0.9/test/test_solar_radiation_pressure_perturbation.py`

 * *Files identical despite different names*

### Comparing `spacestudio-satellite-client-1.0.8/test/test_spacecraft_geometries_api.py` & `spacestudio-satellite-client-1.0.9/test/test_spacecraft_geometries_api.py`

 * *Files identical despite different names*

### Comparing `spacestudio-satellite-client-1.0.8/test/test_spacecraft_geometry.py` & `spacestudio-satellite-client-1.0.9/test/test_spacecraft_geometry.py`

 * *Files identical despite different names*

### Comparing `spacestudio-satellite-client-1.0.8/test/test_studies_api.py` & `spacestudio-satellite-client-1.0.9/test/test_studies_api.py`

 * *Files identical despite different names*

### Comparing `spacestudio-satellite-client-1.0.8/test/test_study.py` & `spacestudio-satellite-client-1.0.9/test/test_study.py`

 * *Files identical despite different names*

### Comparing `spacestudio-satellite-client-1.0.8/test/test_study_computation.py` & `spacestudio-satellite-client-1.0.9/test/test_study_computation.py`

 * *Files identical despite different names*

### Comparing `spacestudio-satellite-client-1.0.8/test/test_study_inputs.py` & `spacestudio-satellite-client-1.0.9/test/test_study_inputs.py`

 * *Files identical despite different names*

### Comparing `spacestudio-satellite-client-1.0.8/test/test_study_parameters.py` & `spacestudio-satellite-client-1.0.9/test/test_study_parameters.py`

 * *Files identical despite different names*

### Comparing `spacestudio-satellite-client-1.0.8/test/test_tab.py` & `spacestudio-satellite-client-1.0.9/test/test_tab.py`

 * *Files identical despite different names*

### Comparing `spacestudio-satellite-client-1.0.8/test/test_third_body_perturbation.py` & `spacestudio-satellite-client-1.0.9/test/test_third_body_perturbation.py`

 * *Files identical despite different names*

### Comparing `spacestudio-satellite-client-1.0.8/test/test_thrust_arcs_position.py` & `spacestudio-satellite-client-1.0.9/test/test_thrust_arcs_position.py`

 * *Files identical despite different names*

### Comparing `spacestudio-satellite-client-1.0.8/test/test_timeline_slot.py` & `spacestudio-satellite-client-1.0.9/test/test_timeline_slot.py`

 * *Files identical despite different names*

