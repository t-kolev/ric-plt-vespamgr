..
.. Copyright (c) 2019 AT&T Intellectual Property.
..
.. Copyright (c) 2019 Nokia.
..
..
.. Licensed under the Creative Commons Attribution 4.0 International
..
.. Public License (the "License"); you may not use this file except
..
.. in compliance with the License. You may obtain a copy of the License at
..
..
..     https://creativecommons.org/licenses/by/4.0/
..
..
.. Unless required by applicable law or agreed to in writing, documentation
..
.. distributed under the License is distributed on an "AS IS" BASIS,
..
.. WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
..
.. See the License for the specific language governing permissions and
..
.. limitations under the License.
..


vespamgr Overview
=================

The VESPA manager uses the VES Agent (https://github.com/nokia/ONAP-VESPA)
to adapt near-RT RIC internal statistics' collection using Prometheus
(xApps and platform containers) to ONAP's VES (VNF event streaming).

The vesmgr container runs two processes: the VESPA manager and the VES Agent (i.s. VESPA).
The VESPA manager starts and configures the VES Agent.
The VES Agent is a service acting as a bridge between Prometheus and ONAP's VES Collector.