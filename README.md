# substrate-metrics-definitions
This is a readme containing all the substrate metrics names, descriptions, and type.

| Name | Description | Type |
| --- | ----------- | --- |
polkadot_memory_allocated | Total bytes allocated by the node | gauge
polkadot_memory_resident | Bytes allocated by the node  and held in RAM | gauge
polkadot_node_is_active_validator | Tracks if the validator is in the active set. Updates at session boundary. | gauge
polkadot_node_is_parachain_validator | Tracks if the validator participates in parachain consensus. Parachain validators are a subset of the active set validators that perform approval checking of all parachain candidates in a session.Updates at session boundary. | gauge
polkadot_parachain_activated_heads_total | Number of activated heads. | counter
polkadot_parachain_approval_candidate_signatures_requests_total | Number of times signatures got requested by other subsystems | counter
polkadot_parachain_approval_checking_finality_lag | How far behind the head of the chain the Approval Checking protocol wants to vote | gauge
polkadot_parachain_approval_distribution_aggression_l1_messages_total | Number of messages in approval distribution for which aggression L1 has been triggered | counter
polkadot_parachain_approval_distribution_aggression_l2_messages_total | Number of messages in approval distribution for which aggression L2 has been triggered | counter
polkadot_parachain_approvals_blockapproval_time_ticks | Number of ticks (500ms) to approve blocks. | histogram
polkadot_parachain_approvals_candidate_approval_time_ticks | Number of ticks (500ms) to approve candidates. | histogram
polkadot_parachain_approvals_imported_total | Number of valid approvals imported locally or from other peers. | counter
polkadot_parachain_approvals_no_shows_total | Number of assignments which became no-shows in the approval voting subsystem | counter
polkadot_parachain_approvals_produced_total | Number of approvals produced by the approval voting subsystem | counter
polkadot_parachain_approvals_wakeups_total | Number of times we woke up to process a candidate in the approval voting subsystem | counter
polkadot_parachain_assignments_imported_total | Number of valid assignments imported locally or from other peers. | counter
polkadot_parachain_assignments_produced | Assignments and tranches produced by the approval voting subsystem | histogram
polkadot_parachain_av_store_block_activated | Time spent within `av_store::process_block_activated` | histogram
polkadot_parachain_av_store_get_chunk | Time spent fetching requested chunks.` | histogram
polkadot_parachain_av_store_process_block_finalized | Time spent within `av_store::process_block_finalized` | histogram
polkadot_parachain_av_store_process_message | Time spent within `av_store::process_message` | histogram
polkadot_parachain_av_store_pruning | Time spent within `av_store::prune_all` | histogram
polkadot_parachain_av_store_store_available_data | Time spent within `av_store::store_available_data` | histogram
polkadot_parachain_av_store_store_chunk | Time spent within `av_store::store_chunk` | histogram
polkadot_parachain_availability_recovery_chunk_requests_finished | Total number of chunk requests finished. | counter
polkadot_parachain_availability_recovery_chunk_requests_issued | Total number of issued chunk requests. | counter
polkadot_parachain_availability_recovery_recoveries_finished | Total number of recoveries that finished. | counter
polkadot_parachain_availability_recovery_recovieries_started | Total number of started recoveries. | counter
polkadot_parachain_availability_recovery_time_chunk_request | Time spent waiting for a response to a chunk request | histogram
polkadot_parachain_availability_recovery_time_erasure_recovery | Time spent to recover the erasure code and verify the merkle root by re-encoding as erasure chunks | histogram
polkadot_parachain_availability_recovery_time_total | Time a full recovery process took  either until failure or successful erasure decoding. | histogram
polkadot_parachain_bitfield_distribution_active_leaves_update | Time spent within `bitfield_distribution::active_leaves_update` | histogram
polkadot_parachain_bitfield_distribution_handle_bitfield_distribution | Time spent within `bitfield_distribution::handle_bitfield_distribution` | histogram
polkadot_parachain_bitfield_distribution_handle_network_msg | Time spent within `bitfield_distribution::handle_network_msg` | histogram
polkadot_parachain_bitfield_signing_run | Time spent within `bitfield_signing::run` | histogram
polkadot_parachain_bitfields_signed_total | Number of bitfields signed. | counter
polkadot_parachain_candidate_backing_candidates_seconded_total | Number of candidates seconded. | counter
polkadot_parachain_candidate_backing_get_backed_candidates | Time spent within `candidate_backing::get_backed_candidates` | histogram
polkadot_parachain_candidate_backing_process_second | Time spent within `candidate_backing::process_second` | histogram
polkadot_parachain_candidate_backing_process_statement | Time spent within `candidate_backing::process_statement` | histogram
polkadot_parachain_candidate_backing_signed_statements_total | Number of statements signed. | counter
polkadot_parachain_candidate_dispute_votes | Accumulated dispute votes  sorted by candidate is `valid` and `invalid`. | counter
polkadot_parachain_candidate_disputes_total | Total number of raised disputes. | counter
polkadot_parachain_candidate_validation_code_size | The size of the decompressed WASM validation blob used for checking a candidate | histogram
polkadot_parachain_candidate_validation_pov_size | The size of the decompressed proof of validity of a candidate | histogram
polkadot_parachain_candidate_validation_validate_candidate_exhaustive | Time spent within `candidate_validation::validate_candidate_exhaustive` | histogram
polkadot_parachain_candidate_validation_validate_from_chain_state | Time spent within `candidate_validation::validate_from_chain_state` | histogram
polkadot_parachain_candidate_validation_validate_from_exhaustive | Time spent within `candidate_validation::validate_from_exhaustive` | histogram
polkadot_parachain_chain_api_ancestors | Time spent within `chain_api::ancestors` | histogram
polkadot_parachain_chain_api_block_headers | Time spent within `chain_api::block_headers` | histogram
polkadot_parachain_chain_api_block_number | Time spent within `chain_api::block_number` | histogram
polkadot_parachain_chain_api_block_weight | Time spent within `chain_api::block_weight` | histogram
polkadot_parachain_chain_api_finalized_block_hash | Time spent within `chain_api::finalized_block_hash` | histogram
polkadot_parachain_chain_api_finalized_block_number | Time spent within `chain_api::finalized_block_number` | histogram
polkadot_parachain_chain_api_requests_total | Number of Chain API requests served. | counter
polkadot_parachain_collation_generation_new_activations | Time spent within fn handle_new_activations | histogram
polkadot_parachain_collation_generation_per_availability_core | Time spent handling a particular availability core for a relay parent in fn handle_new_activations | histogram
polkadot_parachain_collation_generation_per_relay_parent | Time spent handling a particular relay parent within fn handle_new_activations | histogram
polkadot_parachain_collation_requests_total | Number of collations requested from Collators. | counter
polkadot_parachain_collations_generated_total | Number of collations generated. | counter
polkadot_parachain_collator_peer_count | Amount of collator peers connected | gauge
polkadot_parachain_collator_protocol_validator_collation_request_duration | Lifetime of the `PerRequest` structure | histogram
polkadot_parachain_collator_protocol_validator_handle_collation_request_result | Time spent within `collator_protocol_validator::handle_collation_request_result` | histogram
polkadot_parachain_collator_protocol_validator_process_msg | Time spent within `collator_protocol_validator::process_msg` | histogram
polkadot_parachain_deactivated_heads_total | Number of deactivated heads. | counter
polkadot_parachain_desired_peer_count | The number of peers that the local node is expected to connect to on a parachain-related peer-set (either including or not including unresolvable authorities  depending on whether `ConnectToValidators` or `ConnectToValidatorsResolved` was used.) | gauge
polkadot_parachain_dispute_candidate_approval_votes_fetched_total | Number of approval votes fetched from approval voting. | counter
polkadot_parachain_dispute_coordinator_vote_cleanup | Time spent cleaning up old votes per batch. | histogram
polkadot_parachain_dispute_distribution_received_requests | Total number of received dispute requests. | counter
polkadot_parachain_dispute_distribution_time_dispute_request | Time needed for dispute votes to get confirmed/fail getting transmitted. | histogram
polkadot_parachain_dispute_participation_best_effort_queue_size | Number of disputes waiting for local participation in the best effort queue. | gauge
polkadot_parachain_dispute_participation_durations | Time spent within fn Participation::participate | histogram
polkadot_parachain_dispute_participation_pipeline_durations | Measures the duration of the full participation pipeline: From when a participation request is first queued to when participation in the requested dispute is complete. | histogram
polkadot_parachain_dispute_participation_priority_queue_size | Number of disputes waiting for local participation in the priority queue. | gauge
polkadot_parachain_dispute_refrained_participations | Number of refrained participations. We refrain from participation if all of the following conditions are met: disputed candidate is not included  not backed and not confirmed. | counter
polkadot_parachain_disputes_finality_lag | How far behind the head of the chain the Disputes protocol wants to vote | gauge
polkadot_parachain_fetch_retries_total | Number of times we did not succeed in fetching a chunk and needed to try more backers. | counter
polkadot_parachain_fetched_chunks_total | Total number of fetched chunks. | counter
polkadot_parachain_fetched_onchain_disputes | Number of disputes fetched from the runtime | counter
polkadot_parachain_fetched_povs_total | Total number of povs fetches by this backer. | counter
polkadot_parachain_imported_candidates_total | Number of candidates imported by the approval voting subsystem | counter
polkadot_parachain_inherent_data_dispute_statement_sets | Number of dispute statements sets passed to `create_inherent()`. | counter
polkadot_parachain_inherent_data_requests_total | Number of InherentData requests served by provisioner. | counter
polkadot_parachain_messages_relayed_total | Number of messages relayed by Overseer. | counter
polkadot_parachain_network_report_events_total | The amount of reputation changes issued by subsystems | counter
polkadot_parachain_notification_bytes_received_total | The number of bytes received on a parachain notification protocol | counter
polkadot_parachain_notification_bytes_sent_total | The number of bytes sent on a parachain notification protocol | counter
polkadot_parachain_notifications_received_total | The number of notifications received on a parachain protocol | counter
polkadot_parachain_notifications_sent_total | The number of notifications sent on a parachain protocol | counter
polkadot_parachain_overseer_signals_received | Number of signals received by subsystems from overseer | gauge
polkadot_parachain_overseer_signals_sent | Number of signals sent by overseer to subsystems | gauge
polkadot_parachain_peer_connect_events_total | The number of peer connect events on a parachain notifications protocol | counter
polkadot_parachain_peer_count | The number of peers on a parachain-related peer-set | gauge
polkadot_parachain_peer_disconnect_events_total | The number of peer disconnect events on a parachain notifications protocol | counter
polkadot_parachain_provisioner_inherent_data_response_bitfields_sent | Number of inherent bitfields sent in response to `ProvisionerMessage::RequestInherentData`. | histogram
polkadot_parachain_provisioner_partitioned_disputes | Number of disputes partitioned by type. | counter
polkadot_parachain_provisioner_provisionable_data_time | Time spent within `provisioner::provisionable_data` | histogram
polkadot_parachain_provisioner_request_inherent_data_time | Time spent within `provisioner::request_inherent_data` | histogram
polkadot_parachain_received_availability_chunks_total | Number of availability chunks received. | counter
polkadot_parachain_received_availabilty_bitfields_total | Number of valid availability bitfields received from other peers. | counter
polkadot_parachain_runtime_api_make_runtime_api_request | Time spent within `runtime_api::make_runtime_api_request` | histogram
polkadot_parachain_runtime_api_requests_total | Number of Runtime API requests served. | counter
polkadot_parachain_sent_own_availabilty_bitfields_total | Number of own availability bitfields sent to other peers. | counter
polkadot_parachain_served_chunks_total | Total number of chunks served by this backer. | counter
polkadot_parachain_served_povs_total | Total number of povs served by this backer. | counter
polkadot_parachain_statement_distribution_active_leaves_update | Time spent within `statement_distribution::active_leaves_update` | histogram
polkadot_parachain_statement_distribution_created_message_size | Size of created messages containing Seconded statements. | gauge
polkadot_parachain_statement_distribution_network_bridge_update_v1 | Time spent within `statement_distribution::network_bridge_update_v1` | histogram
polkadot_parachain_statement_distribution_sent_requests_total | Number of large statement fetching requests sent. | counter
polkadot_parachain_statement_distribution_share | Time spent within `statement_distribution::share` | histogram
polkadot_parachain_statement_distribution_statements_unexpected | Number of statements that were not expected to be received. | counter
polkadot_parachain_statements_distributed_total | Number of candidate validity statements distributed to other peers. | counter
polkadot_parachain_subsystem_bounded_blocked | Number of times senders blocked while sending messages to a subsystem | gauge
polkadot_parachain_subsystem_bounded_received | Number of elements received by subsystems' bounded queues | gauge
polkadot_parachain_subsystem_bounded_sent | Number of elements sent to subsystems' bounded queues | gauge
polkadot_parachain_subsystem_bounded_tof | Duration spent in a particular channel from entrance to removal | histogram
polkadot_parachain_subsystem_unbounded_received | Number of elements received by subsystems' unbounded queues | gauge
polkadot_parachain_subsystem_unbounded_sent | Number of elements sent to subsystems' unbounded queues | gauge
polkadot_parachain_subsystem_unbounded_tof | Duration spent in a particular channel from entrance to removal | histogram
polkadot_parachain_time_approval_db_transaction | Time spent writing an approval db transaction. | histogram
polkadot_parachain_time_awaiting_approval_voting | Time spent awaiting a reply from the Approval Voting Subsystem. | histogram
polkadot_parachain_time_import_pending_now_known | Time spent on importing pending assignments and approvals. | histogram
polkadot_parachain_time_recover_and_approve | Time spent recovering and approving data in approval voting | histogram
polkadot_parachain_time_unify_with_peer | Time spent within fn `unify_with_peer`. | histogram
polkadot_parachain_unified_with_peer_total | Number of times `unify_with_peer` is called. | counter
polkadot_parachain_validation_requests_total | Number of validation requests served. | counter
polkadot_pvf_execute_enqueued | The total number of jobs enqueued into the execution pipeline | counter
polkadot_pvf_execute_finished | The total number of jobs done in the execution pipeline | counter
polkadot_pvf_execution_time | Time spent in executing PVFs | histogram
polkadot_pvf_precheck_judgement | Time between sending the pre-check request to receiving the response. | histogram
polkadot_pvf_precheck_pvfs_left | The number of PVFs removed from the view. | counter
polkadot_pvf_precheck_pvfs_observed | The number of new PVFs observed. | counter
polkadot_pvf_precheck_votes_duplicate | The number of votes that are submitted more than once for the same code withinthe same session. | counter
polkadot_pvf_precheck_votes_started | The number of votes that are pending submission | counter
polkadot_pvf_precheck_votes_total | The total number of votes submitted. | counter
polkadot_pvf_preparation_max_allocated | max allocated memory observed for preparation (in kilobytes) | histogram
polkadot_pvf_preparation_max_resident | max resident memory observed for preparation (in kilobytes) | histogram
polkadot_pvf_preparation_max_rss | ru_maxrss (maximum resident set size) observed for preparation (in kilobytes) | histogram
polkadot_pvf_preparation_time | Time spent in preparing PVF artifacts in seconds | histogram
polkadot_pvf_prepare_concluded | The total number of jobs concluded in the preparation pipeline | counter
polkadot_pvf_prepare_enqueued | The total number of jobs enqueued into the preparation pipeline | counter
polkadot_pvf_worker_spawned | The total number of workers spawned successfully | counter
polkadot_pvf_worker_spawning | The total number of workers began to spawn | counter
substrate_authority_discovery_amount_external_addresses_last_published | Number of external addresses published when authority discovery last published addresses. | gauge
substrate_authority_discovery_authority_address_requests_pending | Number of pending authority address requests. | gauge
substrate_authority_discovery_authority_addresses_requested_total | Number of times authority discovery has requested external addresses of a single authority. | counter
substrate_authority_discovery_dht_event_received | Number of dht events received by authority discovery. | counter
substrate_authority_discovery_handle_value_found_event_failure | Number of times handling a dht value found event failed. | counter
substrate_authority_discovery_known_authorities_count | Number of authorities known by authority discovery. | gauge
substrate_authority_discovery_times_published_total | Number of times authority discovery has published external addresses. | counter
substrate_beefy_bad_justification_imports | Number of bad justifications on block-import | counter
substrate_beefy_failed_justification_responses | Number of Failed Justification responses | counter
substrate_beefy_good_justification_imports | Number of good justifications on block-import | counter
substrate_beefy_successful_justification_responses | Number of Successful Justification responses | counter
substrate_block_height | Block height info of the chain | gauge
substrate_block_verification_and_import_time | Time taken to verify and import blocks | histogram
substrate_block_verification_time | Time taken to verify blocks | histogram
substrate_build_info | A metric with a constant '1' value labeled by name  version | gauge
substrate_database_cache_bytes | RocksDB cache size in bytes | gauge
substrate_finality_grandpa_communication_gossip_validator_messages | Number of messages validated by the finality grandpa gossip validator. | counter
substrate_finality_grandpa_precommits_total | Total number of GRANDPA precommits cast locally. | counter
substrate_finality_grandpa_prevotes_total | Total number of GRANDPA prevotes cast locally. | counter
substrate_finality_grandpa_round | Highest completed GRANDPA round. | gauge
substrate_finality_grandpa_until_imported_waiting_messages_number | Number of finality grandpa messages waiting within the until imported queue. | gauge
substrate_import_queue_processed_total | Blocks processed by import queue | counter
substrate_issued_light_requests | Number of light client requests that our node has issued. | counter
substrate_justification_import_time | Time taken to import justifications | histogram
substrate_network_gossip_expired_messages_total | Number of expired messages by the gossip service. | counter
substrate_network_gossip_registered_messages_total | Number of registered messages by the gossip service. | counter
substrate_node_roles | The roles the node is running as | gauge
substrate_number_leaves | Number of known chain leaves (aka forks) | gauge
substrate_process_start_time_seconds | Number of seconds between the UNIX epoch and the moment the process started | gauge
substrate_proposer_block_constructed | Histogram of time taken to construct new block | histogram
substrate_proposer_block_proposal_time | Histogram of time taken to construct a block and prepare it for proposal | histogram
substrate_proposer_create_inherents_time | Histogram of time taken to execute create inherents | histogram
substrate_proposer_end_proposal_reason | The reason why the block proposing was ended. This doesn't include errors. | counter
substrate_proposer_number_of_transactions | Number of transactions included in block | gauge
substrate_ready_transactions_number | Number of transactions in the ready queue | gauge
substrate_rpc_calls_finished | Number of processed RPC calls (unique un-batched requests) | counter
substrate_rpc_calls_started | Number of received RPC calls (unique un-batched requests) | counter
substrate_rpc_calls_time | Total time [μs] of processed RPC calls | histogram
substrate_rpc_requests_finished | Number of RPC requests (not calls) processed by the server. | counter
substrate_rpc_requests_started | Number of RPC requests (not calls) received by the server. | counter
substrate_rpc_sessions_closed | Number of persistent RPC sessions closed | counter
substrate_rpc_sessions_opened | Number of persistent RPC sessions opened | counter
substrate_state_cache_bytes | State cache size in bytes | gauge
substrate_sub_libp2p_connections_closed_total | Total number of connections closed  by direction and reason | counter
substrate_sub_libp2p_connections_opened_total | Total number of connections opened by direction | counter
substrate_sub_libp2p_distinct_peers_connections_closed_total | Total number of connections closed with distinct peers | counter
substrate_sub_libp2p_distinct_peers_connections_opened_total | Total number of connections opened with distinct peers | counter
substrate_sub_libp2p_incoming_connections_handshake_errors_total | Total number of incoming connections that have failed during the initial handshake | counter
substrate_sub_libp2p_incoming_connections_total | Total number of incoming connections on the listening sockets | counter
substrate_sub_libp2p_is_major_syncing | Whether the node is performing a major sync or not. | gauge
substrate_sub_libp2p_kademlia_query_duration | Duration of Kademlia queries per query type | histogram
substrate_sub_libp2p_kademlia_random_queries_total | Number of random Kademlia queries started | counter
substrate_sub_libp2p_kademlia_records_count | Number of records in the Kademlia records store | gauge
substrate_sub_libp2p_kademlia_records_sizes_total | Total size of all the records in the Kademlia records store | gauge
substrate_sub_libp2p_kbuckets_num_nodes | Number of nodes per kbucket per Kademlia instance | gauge
substrate_sub_libp2p_listeners_errors_total | Total number of non-fatal errors reported by a listener | counter
substrate_sub_libp2p_listeners_local_addresses | Number of local addresses we're listening on | gauge
substrate_sub_libp2p_network_bytes_total | Total bandwidth usage | counter
substrate_sub_libp2p_notifications_sizes | Sizes of the notifications send to and received from all nodes | histogram
substrate_sub_libp2p_notifications_streams_closed_total | Total number of notification substreams that have been closed | counter
substrate_sub_libp2p_notifications_streams_opened_total | Total number of notification substreams that have been opened | counter
substrate_sub_libp2p_out_events_events_total | Number of broadcast network events that have been sent or received across all channels | counter
substrate_sub_libp2p_out_events_notifications_sizes | Size of notification events that have been sent or received across all channels | counter
substrate_sub_libp2p_out_events_num_channels | Number of internal active channels that broadcast network events | gauge
substrate_sub_libp2p_peers_count | Number of connected peers | gauge
substrate_sub_libp2p_peerset_num_discovered | Number of nodes stored in the peerset manager | gauge
substrate_sub_libp2p_pending_connections | Number of connections in the process of being established | gauge
substrate_sub_libp2p_pending_connections_errors_total | Total number of pending connection errors | counter
substrate_sub_libp2p_requests_in_success_total | For successful incoming requests  time between receiving the request and starting to send the response | histogram
substrate_sub_libp2p_requests_out_failure_total | Total number of requests that have failed | counter
substrate_sub_libp2p_requests_out_success_total | For successful outgoing requests  time between a request's start and finish | histogram
substrate_sub_txpool_block_transactions_pruned | Total number of transactions that was requested to be pruned by block events | counter
substrate_sub_txpool_block_transactions_resubmitted | Total number of transactions that was requested to be resubmitted by block events | counter
substrate_sub_txpool_submitted_transactions | Total number of transactions submitted | counter
substrate_sub_txpool_validations_finished | Total number of transactions that finished validation | counter
substrate_sub_txpool_validations_invalid | Total number of transactions that were removed from the pool as invalid | counter
substrate_sub_txpool_validations_scheduled | Total number of transactions scheduled for validation | counter
substrate_sync_extra_justifications | Number of extra justifications requests | gauge
substrate_sync_fork_targets | Number of fork sync targets | gauge
substrate_sync_import_queue_blocks_submitted | Number of blocks submitted to the import queue. | counter
substrate_sync_import_queue_justifications_submitted | Number of justifications submitted to the import queue. | counter
substrate_sync_peers | Number of peers we sync with | gauge
substrate_sync_propagated_transactions | Number of transactions propagated to at least one peer | counter
substrate_sync_queued_blocks | Number of blocks in import queue | gauge
substrate_tasks_ended_total | Total number of tasks for which Future::poll has returned Ready(()) or panicked | counter
substrate_tasks_polling_duration | Duration in seconds of each invocation of Future::poll | histogram
substrate_tasks_polling_started_total | Total number of times we started invoking Future::poll | counter
substrate_tasks_spawned_total | Total number of tasks that have been spawned on the Service | counter
substrate_tokio_threads_alive | Number of threads alive right now | gauge
substrate_tokio_threads_total | Total number of threads created | counter
substrate_unbounded_channel_len | Items in each mpsc::unbounded instance | counter
