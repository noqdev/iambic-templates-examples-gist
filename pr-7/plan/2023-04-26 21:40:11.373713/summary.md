# IAMbic Summary
## Change Detection
* 4 distinct actions.
* 4 templates with changes.
* 4 accounts affected.
## Exceptions
* 0 exceptions were recorded.

# IAMbic Change Details

<details>
<summary>Action: Create (Number of Templates: 1)</summary>
    <blockquote>
        <details>
        <summary>Template: iambic_test_role.yaml (Number of Accounts: 4)</summary>
            <blockquote>
                <details>
                <summary>Account: iambic_test_spoke_account_1 - (442632209887) (Number of Changes: 1)</summary>
                    <blockquote>
                        <table>
                            <thead>
                                <tr>
                                    <th>Resource ID</th>
                                    <th>Resource Type</th>
                                    <th>Change Type</th>
                                </tr>
                            </thead>
                            <tbody>
                                <tr>
                                    <td>s3-access</td>
                                    <td>aws:policy_document</td>
                                    <td>Create</td>
                                </tr>
                                </tbody>
                        </table>
                        </blockquote>
                </details>
                <details>
                <summary>Account: iambic_test_spoke_account_3 - (333972133479) (Number of Changes: 1)</summary>
                    <blockquote>
                        <table>
                            <thead>
                                <tr>
                                    <th>Resource ID</th>
                                    <th>Resource Type</th>
                                    <th>Change Type</th>
                                </tr>
                            </thead>
                            <tbody>
                                <tr>
                                    <td>s3-access</td>
                                    <td>aws:policy_document</td>
                                    <td>Create</td>
                                </tr>
                                </tbody>
                        </table>
                        </blockquote>
                </details>
                <details>
                <summary>Account: iambic_test_org_account - (580605962305) (Number of Changes: 1)</summary>
                    <blockquote>
                        <table>
                            <thead>
                                <tr>
                                    <th>Resource ID</th>
                                    <th>Resource Type</th>
                                    <th>Change Type</th>
                                </tr>
                            </thead>
                            <tbody>
                                <tr>
                                    <td>s3-access</td>
                                    <td>aws:policy_document</td>
                                    <td>Create</td>
                                </tr>
                                </tbody>
                        </table>
                        </blockquote>
                </details>
                <details>
                <summary>Account: iambic_test_spoke_account_2 - (192455039954) (Number of Changes: 1)</summary>
                    <blockquote>
                        <table>
                            <thead>
                                <tr>
                                    <th>Resource ID</th>
                                    <th>Resource Type</th>
                                    <th>Change Type</th>
                                </tr>
                            </thead>
                            <tbody>
                                <tr>
                                    <td>s3-access</td>
                                    <td>aws:policy_document</td>
                                    <td>Create</td>
                                </tr>
                                </tbody>
                        </table>
                        </blockquote>
                </details>
                </blockquote>
        </details>
        </blockquote>
</details>
<details>
<summary>Action: Delete (Number of Templates: 1)</summary>
    <blockquote>
        <details>
        <summary>Template: iambic_test_role.yaml (Number of Accounts: 4)</summary>
            <blockquote>
                <details>
                <summary>Account: iambic_test_spoke_account_1 - (442632209887) (Number of Changes: 1)</summary>
                    <blockquote>
                        <table>
                            <thead>
                                <tr>
                                    <th>Resource ID</th>
                                    <th>Resource Type</th>
                                    <th>Change Type</th>
                                </tr>
                            </thead>
                            <tbody>
                                <tr>
                                    <td>spoke-acct-policy</td>
                                    <td>aws:policy_document</td>
                                    <td>Delete</td>
                                </tr>
                                </tbody>
                        </table>
                        </blockquote>
                </details>
                <details>
                <summary>Account: iambic_test_spoke_account_3 - (333972133479) (Number of Changes: 1)</summary>
                    <blockquote>
                        <table>
                            <thead>
                                <tr>
                                    <th>Resource ID</th>
                                    <th>Resource Type</th>
                                    <th>Change Type</th>
                                </tr>
                            </thead>
                            <tbody>
                                <tr>
                                    <td>spoke-acct-policy</td>
                                    <td>aws:policy_document</td>
                                    <td>Delete</td>
                                </tr>
                                </tbody>
                        </table>
                        </blockquote>
                </details>
                <details>
                <summary>Account: iambic_test_org_account - (580605962305) (Number of Changes: 1)</summary>
                    <blockquote>
                        <table>
                            <thead>
                                <tr>
                                    <th>Resource ID</th>
                                    <th>Resource Type</th>
                                    <th>Change Type</th>
                                </tr>
                            </thead>
                            <tbody>
                                <tr>
                                    <td>spoke-acct-policy</td>
                                    <td>aws:policy_document</td>
                                    <td>Delete</td>
                                </tr>
                                </tbody>
                        </table>
                        </blockquote>
                </details>
                <details>
                <summary>Account: iambic_test_spoke_account_2 - (192455039954) (Number of Changes: 1)</summary>
                    <blockquote>
                        <table>
                            <thead>
                                <tr>
                                    <th>Resource ID</th>
                                    <th>Resource Type</th>
                                    <th>Change Type</th>
                                </tr>
                            </thead>
                            <tbody>
                                <tr>
                                    <td>spoke-acct-policy</td>
                                    <td>aws:policy_document</td>
                                    <td>Delete</td>
                                </tr>
                                </tbody>
                        </table>
                        </blockquote>
                </details>
                </blockquote>
        </details>
        </blockquote>
</details>
<details>
<summary>Action: Attach (Number of Templates: 1)</summary>
    <blockquote>
        <details>
        <summary>Template: iambic_test_role.yaml (Number of Accounts: 4)</summary>
            <blockquote>
                <details>
                <summary>Account: iambic_test_spoke_account_1 - (442632209887) (Number of Changes: 2)</summary>
                    <blockquote>
                        <table>
                            <thead>
                                <tr>
                                    <th>Resource ID</th>
                                    <th>Resource Type</th>
                                    <th>Change Type</th>
                                </tr>
                            </thead>
                            <tbody>
                                <tr>
                                    <td>arn:aws:iam::aws:policy/AmazonS3ReadOnlyAccess</td>
                                    <td>aws:policy_document</td>
                                    <td>Attach</td>
                                </tr>
                                </tbody>
                        </table>
                        <table>
                            <thead>
                                <tr>
                                    <th>Resource ID</th>
                                    <th>Resource Type</th>
                                    <th>Change Type</th>
                                </tr>
                            </thead>
                            <tbody>
                                <tr>
                                    <td>arn:aws:iam::aws:policy/job-function/SupportUser</td>
                                    <td>aws:policy_document</td>
                                    <td>Attach</td>
                                </tr>
                                </tbody>
                        </table>
                        </blockquote>
                </details>
                <details>
                <summary>Account: iambic_test_spoke_account_3 - (333972133479) (Number of Changes: 2)</summary>
                    <blockquote>
                        <table>
                            <thead>
                                <tr>
                                    <th>Resource ID</th>
                                    <th>Resource Type</th>
                                    <th>Change Type</th>
                                </tr>
                            </thead>
                            <tbody>
                                <tr>
                                    <td>arn:aws:iam::aws:policy/AmazonS3ReadOnlyAccess</td>
                                    <td>aws:policy_document</td>
                                    <td>Attach</td>
                                </tr>
                                </tbody>
                        </table>
                        <table>
                            <thead>
                                <tr>
                                    <th>Resource ID</th>
                                    <th>Resource Type</th>
                                    <th>Change Type</th>
                                </tr>
                            </thead>
                            <tbody>
                                <tr>
                                    <td>arn:aws:iam::aws:policy/job-function/SupportUser</td>
                                    <td>aws:policy_document</td>
                                    <td>Attach</td>
                                </tr>
                                </tbody>
                        </table>
                        </blockquote>
                </details>
                <details>
                <summary>Account: iambic_test_org_account - (580605962305) (Number of Changes: 2)</summary>
                    <blockquote>
                        <table>
                            <thead>
                                <tr>
                                    <th>Resource ID</th>
                                    <th>Resource Type</th>
                                    <th>Change Type</th>
                                </tr>
                            </thead>
                            <tbody>
                                <tr>
                                    <td>arn:aws:iam::aws:policy/AmazonS3ReadOnlyAccess</td>
                                    <td>aws:policy_document</td>
                                    <td>Attach</td>
                                </tr>
                                </tbody>
                        </table>
                        <table>
                            <thead>
                                <tr>
                                    <th>Resource ID</th>
                                    <th>Resource Type</th>
                                    <th>Change Type</th>
                                </tr>
                            </thead>
                            <tbody>
                                <tr>
                                    <td>arn:aws:iam::aws:policy/job-function/SupportUser</td>
                                    <td>aws:policy_document</td>
                                    <td>Attach</td>
                                </tr>
                                </tbody>
                        </table>
                        </blockquote>
                </details>
                <details>
                <summary>Account: iambic_test_spoke_account_2 - (192455039954) (Number of Changes: 2)</summary>
                    <blockquote>
                        <table>
                            <thead>
                                <tr>
                                    <th>Resource ID</th>
                                    <th>Resource Type</th>
                                    <th>Change Type</th>
                                </tr>
                            </thead>
                            <tbody>
                                <tr>
                                    <td>arn:aws:iam::aws:policy/AmazonS3ReadOnlyAccess</td>
                                    <td>aws:policy_document</td>
                                    <td>Attach</td>
                                </tr>
                                </tbody>
                        </table>
                        <table>
                            <thead>
                                <tr>
                                    <th>Resource ID</th>
                                    <th>Resource Type</th>
                                    <th>Change Type</th>
                                </tr>
                            </thead>
                            <tbody>
                                <tr>
                                    <td>arn:aws:iam::aws:policy/job-function/SupportUser</td>
                                    <td>aws:policy_document</td>
                                    <td>Attach</td>
                                </tr>
                                </tbody>
                        </table>
                        </blockquote>
                </details>
                </blockquote>
        </details>
        </blockquote>
</details>
<details>
<summary>Action: Detach (Number of Templates: 1)</summary>
    <blockquote>
        <details>
        <summary>Template: iambic_test_role.yaml (Number of Accounts: 4)</summary>
            <blockquote>
                <details>
                <summary>Account: iambic_test_spoke_account_1 - (442632209887) (Number of Changes: 1)</summary>
                    <blockquote>
                        <table>
                            <thead>
                                <tr>
                                    <th>Resource ID</th>
                                    <th>Resource Type</th>
                                    <th>Change Type</th>
                                </tr>
                            </thead>
                            <tbody>
                                <tr>
                                    <td>arn:aws:iam::aws:policy/job-function/ViewOnlyAccess</td>
                                    <td>aws:policy_document</td>
                                    <td>Detach</td>
                                </tr>
                                </tbody>
                        </table>
                        </blockquote>
                </details>
                <details>
                <summary>Account: iambic_test_spoke_account_3 - (333972133479) (Number of Changes: 1)</summary>
                    <blockquote>
                        <table>
                            <thead>
                                <tr>
                                    <th>Resource ID</th>
                                    <th>Resource Type</th>
                                    <th>Change Type</th>
                                </tr>
                            </thead>
                            <tbody>
                                <tr>
                                    <td>arn:aws:iam::aws:policy/job-function/ViewOnlyAccess</td>
                                    <td>aws:policy_document</td>
                                    <td>Detach</td>
                                </tr>
                                </tbody>
                        </table>
                        </blockquote>
                </details>
                <details>
                <summary>Account: iambic_test_org_account - (580605962305) (Number of Changes: 1)</summary>
                    <blockquote>
                        <table>
                            <thead>
                                <tr>
                                    <th>Resource ID</th>
                                    <th>Resource Type</th>
                                    <th>Change Type</th>
                                </tr>
                            </thead>
                            <tbody>
                                <tr>
                                    <td>arn:aws:iam::aws:policy/job-function/ViewOnlyAccess</td>
                                    <td>aws:policy_document</td>
                                    <td>Detach</td>
                                </tr>
                                </tbody>
                        </table>
                        </blockquote>
                </details>
                <details>
                <summary>Account: iambic_test_spoke_account_2 - (192455039954) (Number of Changes: 1)</summary>
                    <blockquote>
                        <table>
                            <thead>
                                <tr>
                                    <th>Resource ID</th>
                                    <th>Resource Type</th>
                                    <th>Change Type</th>
                                </tr>
                            </thead>
                            <tbody>
                                <tr>
                                    <td>arn:aws:iam::aws:policy/job-function/ViewOnlyAccess</td>
                                    <td>aws:policy_document</td>
                                    <td>Detach</td>
                                </tr>
                                </tbody>
                        </table>
                        </blockquote>
                </details>
                </blockquote>
        </details>
        </blockquote>
</details>

